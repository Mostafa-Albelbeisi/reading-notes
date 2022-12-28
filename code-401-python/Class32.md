# Next Js
The easiest way to get started with **Next.js** is by using create-next-app. This CLI tool enables you to quickly start building a new Next.js application, with everything set up for you. You can create a new app using the default Next.js template, or by using one of the official **Next.js** examples. To get started, use the following command: `npx create-next-app@latest`

## Why use Create Next App?
create-next-app allows you to create a new Next.js app within seconds. It is officially maintained by the creators of Next.js, and includes a number of **benefits**:

- **Interactive Experience:** Running npx create-next-app@latest (with no arguments) launches an interactive experience that guides you through setting up a project.
- **Zero Dependencies:** Initializing a project is as quick as one second. Create Next App has zero dependencies.
- **Offline Support:** Create Next App will automatically detect if you're offline and bootstrap your project using your local package cache.
- **Support for Examples:** Create Next App can bootstrap your application using an example from the Next.js examples collection (e.g. npx create-next-app --example api-routes).
- **Tested:** The package is part of the Next.js monorepo and tested using the same integration test suite as Next.js itself, ensuring it works as expected with every release.



# Tailwind CSS
**Tailwind** CSS is an open source CSS framework. The main feature of this library is that, unlike other CSS frameworks like Bootstrap, it does not provide a series of predefined classes for elements such as buttons or tables.

All of the components in Tailwind UI are designed for the latest version of Tailwind CSS, which is currently Tailwind CSS v3.2. To make sure that you are on the latest version of Tailwind, update via npm: `npm install tailwindcss@latest`

## But once you’ve actually built something this way, you’ll quickly notice some really important benefits:

- **You aren’t wasting energy inventing class names.** No more adding silly class names like sidebar-inner-wrapper just to be able to style something, and no more agonizing over the perfect abstract name for something that’s really just a flex container.
- **Your CSS stops growing.** Using a traditional approach, your CSS files get bigger every time you add a new feature. With utilities, everything is reusable so you rarely need to write new CSS.
- **Making changes feels safer.** CSS is global and you never know what you’re breaking when you make a change. Classes in your HTML are local, so you can change them without worrying about something else breaking.

## But using utility classes has a few important advantages over inline styles:

- **Designing with constraints.** Using inline styles, every value is a magic number. With utilities, you’re choosing styles from a predefined design system, which makes it much easier to build visually consistent UIs.
- **Responsive design.** You can’t use media queries in inline styles, but you can use Tailwind’s **responsive utilities** to build fully responsive interfaces easily.
- **Hover, focus, and other states.** Inline styles can’t target states like hover or focus, but Tailwind’s state variants make it easy to style those states with utility classes.


# Creating components
All React examples are provided as a simple single component and make no assumptions about how you want to break things down, what prop APIs you want to expose, or where you get any data from.

Some data has been extracted into basic local variables just to clean up duplication and make the code easier to read and understand, but we've tried to do as little as possible to avoid enforcing any unnecessarily rigid opinions.

When you're adapting code from Tailwind UI for your own projects, you should break the examples down into smaller components as necessary to achieve whatever level of reuse you need for your project.

For example, you might start with this stacked list component:

        const people = [
        {
            name: 'Calvin Hawkins',
            email: 'calvin.hawkins@example.com',
            image:
            'https://images.unsplash.com/photo-1491528323818-fdd1faba62cc?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=256&h=256&q=80',
        },
        {
            name: 'Kristen Ramos',
            email: 'kristen.ramos@example.com',
            image:
            'https://images.unsplash.com/photo-1550525811-e5869dd03032?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=256&h=256&q=80',
        },
        {
            name: 'Ted Fox',
            email: 'ted.fox@example.com',
            image:
            'https://images.unsplash.com/photo-1500648767791-00dcc994a43e?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=256&h=256&q=80',
        },
        ]

        export default function Example() {
        return (
            <ul className="divide-y divide-gray-200">
            {people.map((person) => (
                <li key={person.email} className="py-4 flex">
                <img className="h-10 w-10 rounded-full" src={person.image} alt="" />
                <div className="ml-3">
                    <p className="text-sm font-medium text-gray-900">{person.name}</p>
                    <p className="text-sm text-gray-500">{person.email}</p>
                </div>
                </li>
            ))}
            </ul>
        )
        }

