# DRF Permissions

Permissions in REST framework are always defined as a list of permission classes.

### When the permission checks fail, either a "403 Forbidden" or a "401 Unauthorized" response will be returned, according to the following rules:

* The request was successfully authenticated, but permission was denied. — An HTTP 403 Forbidden response will be returned.
* The request was not successfully authenticated, and the highest priority authentication class does not use WWW-Authenticate headers. — An HTTP 403 Forbidden response will be returned.
* The request was not successfully authenticated, and the highest priority authentication class does use WWW-Authenticate headers. — An HTTP 401 Unauthorized response, with an appropriate WWW-Authenticate header will be returned.


# Generic views
**Django’s generic views**... were developed as a shortcut for common usage patterns... They take certain common idioms and patterns found in view development and abstract them so that you can quickly write common views of data without having to repeat yourself.

### Basic settings:

The following attributes control the basic view behavior.

- `**queryset**` - The queryset that should be used for returning objects from this view. Typically, you must either set this attribute, or override the ``get_queryset()`` method. If you are overriding a view method, it is important that you call ``get_queryset()`` instead of accessing this property directly, as `queryset` will get evaluated once, and those results will be cached for all subsequent requests.
- `serializer_class` - The serializer class that should be used for validating and deserializing input, and for serializing output. Typically, you must either set this attribute, or override the `get_serializer_class()` method.
- `lookup_field` - The model field that should be used for performing object lookup of individual model instances. Defaults to `'pk'`. Note that when using hyperlinked APIs you'll need to ensure that both the API views and the serializer classes set the lookup fields if you need to use a custom value.
- `lookup_url_kwarg` - The URL keyword argument that should be used for object lookup. The URL conf should include a keyword argument corresponding to this value. If unset this defaults to using the same value as lookup_field.

### Pagination:
* `pagination_class` - The pagination class that should be used when paginating list results. Defaults to the same value as the `DEFAULT_PAGINATION_CLASS` setting, which is '`rest_framework.pagination.PageNumberPagination`'. Setting `pagination_class=None` will disable pagination on this view.

### Filtering:
* `filter_backends` - A list of filter backend classes that should be used for filtering the queryset. Defaults to the same value as the `DEFAULT_FILTER_BACKENDS` setting.


# API Reference
## AllowAny
The `AllowAny` permission class will allow unrestricted access, regardless of if the request was authenticated or unauthenticated.

This permission is not strictly required, since you can achieve the same result by using an empty list or tuple for the permissions setting, but you may find it useful to specify this class because it makes the intention explicit.

## IsAuthenticated
The `IsAuthenticated` permission class will deny permission to any unauthenticated user, and allow permission otherwise.

This permission is suitable if you want your API to only be accessible to registered users.

## IsAdminUser
The `IsAdminUser` permission class will deny permission to any user, unless user.is_staff is True in which case permission will be allowed.

This permission is suitable if you want your API to only be accessible to a subset of trusted administrators.

## IsAuthenticatedOrReadOnly
The `IsAuthenticatedOrReadOnly` will allow authenticated users to perform any request. Requests for unauthorised users will only be permitted if the request method is one of the "safe" methods; GET, HEAD or OPTIONS.

This permission is suitable if you want to your API to allow read permissions to anonymous users, and only allow write permissions to authenticated users.

## DjangoModelPermissions
This permission class ties into Django's `standard django.contrib.auth` model permissions. This permission must only be applied to views that have a `.queryset` property or `get_queryset()` method. Authorization will only be granted if the user is authenticated and has the relevant model permissions assigned. The appropriate model is determined by checking `get_queryset().model` or `queryset.model`.

* `POST` requests require the user to have the `add` permission on the model.
* `PUT` and `PATCH` requests require the user to have the `change` permission on the model.
* `DELETE` requests require the user to have the `delete` permission on the model.
The default behaviour can also be overridden to support custom model permissions. For example, you might want to include a `view` model permission for `GET` requests.

To use custom model permissions, override `DjangoModelPermissions` and set the `.perms_map` property. Refer to the source code for details.