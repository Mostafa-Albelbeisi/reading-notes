# Authentication

## What is authentication?
**Authentication** is the process of determining whether someone or something is, in fact, who or what it says it is. Authentication technology provides access control for systems by checking to see if a user's credentials match the credentials in a database of authorized users or in a data authentication server. In doing this, authentication assures secure systems, secure processes and enterprise information security.

## Why is authentication important in cybersecurity?
Authentication enables organizations to keep their networks secure by permitting only authenticated users or processes to gain access to their protected resources. This may include computer systems, networks, databases, websites and other network-based applications or services.


## What is authentication used for?
User and process authentication are used to ensure that only authorized individuals or processes are allowed to access company IT resources. Depending on the use cases for which authentication is used, authentication can consist of either SFA, 2FA or MFA.

## What are authentication factors?
Authenticating a user with a user ID and a password is usually considered the most basic type of authentication, and it depends on the user knowing two pieces of information -- the user ID or username, and the password. Since this type of authentication relies on just one authentication factor, it is a type of SFA.


### Currently used authentication factors include the following:

* **Knowledge factor**. The knowledge factor, or something you know, may be any authentication credentials that consist of information that the user possesses, including a personal identification number (PIN), a username, a password or the answer to a secret question.
* **Possession factor**. The possession factor, or something you have, may be any credential based on items that the user can own and carry with them, including hardware devices, like a security token or a mobile phone used to accept a text message or to run an authentication app that can generate a one-time password (OTP) or PIN.
* **Inherence factor**. The inherence factor, or something you are, is typically based on some form of biometric identification, including fingerprints or thumbprints, facial recognition, retina scan or any other form of biometric data.
* **Location factor**. Where you are may be less specific, but the location factor is sometimes used as an adjunct to the other factors. Location can be determined to reasonable accuracy by devices equipped with the Global Positioning System or with less accuracy by checking network addresses and routes. The location factor cannot usually stand on its own for authentication, but it can supplement the other factors by providing a means of ruling out some requests. For example, it can prevent an attacker located in a remote geographical area from posing as a user who normally logs in only from their home or office in the organization's home country.
* **Time factor**. Like the location factor, the time factor, or when you are authenticating, is not sufficient on its own, but it can be a supplemental mechanism for weeding out attackers who attempt to access a resource at a time when that resource is not available to the authorized user. It may also be used together with location. For example, if the user was last authenticated at noon in the U.S., an attempt to authenticate from Asia one hour later would be rejected based on the combination of time and location.


## Authentication vs. authorization
**Authorization** includes the process through which an administrator grants rights to **authenticated** users, as well as the process of checking user account permissions to verify that the user has been granted access to those resources. The privileges and preferences granted for an authorized account depend on the user's permissions, which are either stored locally or on an authentication server. The settings defined for all these environment variables are established by an administrator.