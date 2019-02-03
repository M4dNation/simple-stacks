# simple-stacks

[![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
[![npm version](https://badge.fury.io/js/simple-stacks.svg)](https://badge.fury.io/js/simple-stacks)
[![Build Status](https://travis-ci.org/M4dNation/simple-stacks.png?branch=master)](https://travis-ci.org/M4dNation/simple-stacks) ![](https://david-dm.org/M4dNation/simple-stacks.svg) [![codecov](https://codecov.io/gh/M4dNation/simple-stacks/branch/develop/graph/badge.svg)](https://codecov.io/gh/M4dNation/simple-stacks)

## About

`simple-stacks` is a package for creating a stack structure.  
It provides one `Stack` class you can instanciate and populate with any data you want.

## Install

`npm install --save simple-stacks`  
`yarn add simple-stacks`

## Usage

`simple-stacks` exports a `Stack` class you can import:

```javascript
// ES6
import { Stack } from "simple-stacks";

// ES5
const Stack = require("simple-stacks").Stack;
```

Once imported, you just have to instanciate a Stack and add data to have an usable stack.

```javascript
import { Stack } from "simple-stacks";

const stack = new Stack();
const myData = { id: "some-id" };

stack.push(myData);
stack.push("test1");

stack.pop();
```

## Authors

`simple-stacks` is maintained by M4dNation Company.  
First version written by [axelvaindal](https://github.com/axelvaindal).

## Contributors

There is actually no other contributors for this project.
If you want to contribute, feel free to make any suggestions or to contact us.

### Contributing to the package

We try to keep `simple-stacks` as simple as possible.  
Before proposing a PR or opening an issue, please keep in mind :

    - This package is meant to be as simple as possible
    - This package tries to respect the [Single Responsibility Principle](https://en.wikipedia.org/wiki/Single_responsibility_principle)
    - This package tries to use the minimum of dependencies possible

Taking into account the previous points leads us to **NOT** merge proposed pull-request if those :

    - Integrate changes that are too far from the initial purpose of the package
    - Integrate changes that are adding additional dependencies
    - Integrate changes that are not unit tested and motivationated

This being said, we **really** welcome pull-request and bug report, so feel free to start a contribution.

Moreover, Pull Requests should always come with related unit tests, and won't be considered if tests aren't included.

### Testing

`simple-stacks` uses jest for unit testing.  
If you don't know about jest yet, you can check out their [documentation](https://jestjs.io/en/).

To run the tests, just run :

`yarn test`

Note that we are using [codecov](https://codecov.io) to keep track of code coverage related to our tests and you shouldn't affect negatively the current coverage of the code by removing tests or not covering new features with new unit tests.

## Licence

`simple-stacks` is available under the terms of the MIT LICENSE.  
Check the licence file for more information.
