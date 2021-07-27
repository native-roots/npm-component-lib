# Native Roots NPM Shared Component Library

A library of shared components across Native Roots Web Apps

## How to use

Fork this repo, clone it to your local computer, and edit the `package.json` along with every other required file to match your project.
Write the code for your package in TypeScript and Sass, compile it, and publish it to [npm](https://npmjs.com).

To compile your code once, run

- `npm run build`.

To compile your code once and refresh on file change, run

- `npm run start`.

To publish your package to npm, make sure you're logged in the correct account by running

- `npm login`.

Compile your package by running

- `npm run build`

Update the package version accordingly by using

- [`npm version [patch | minor | major]`](https://docs.npmjs.com/about-semantic-versioning)

Then publish your package by running

- `npm publish`



## Using this package locally (not directly from the NPM Directory)

Start by running `npm run build` from the root of this project

Then run `npm link` to setup the local linking mechanism

Run `npm link /path/to/project/we/want/to/use/this/lib/in/node_modules/react` from the root of this directory. 
It is a necessary command to ensure that this package and the project we intend to use it in are on the same version of React

Run `npm link npm-component-lib` in the root of the project that we want to use this package in.

Import the components in that project and use accordingly.