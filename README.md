# ARK Development Guidelines

## Introduction

While the following guidelines are not an absolute requirement or need to be enforced by tools, it is a recommendation based on what we have been doing in our projects lately.

## How to approach `JavaScript` projects

### Directory Structure

* `lib/` is intended for code that can run as-is with `require()`.
* `src/` is intended for code that needs to be build with webpack before it can be used.
* `build/` is for webpack scripts needed to build your project.
* `dist/` is for compiled modules that can be used with other systems.
* `bin/` is for any executable scripts, or compiled binaries used with, or built from your module.
* `__tests__/` is for all of your tests with [jest](https://github.com/facebook/jest).

#### lib

If you are developing a module only for server-side use with node.js all files should be placed in the `lib` directory.

#### src

If you are developing a module for server-side and/or browser use all files should be placed in the `src` directory.

#### build

If you are building a module that needs to run both in the browser and on a server you should use [webpack](https://github.com/webpack/webpack) and place the build scripts inside the `build` directory.

#### dist

If your module is to be built for use with other platforms through webpack, the output should be placed in the `dist` directory.

#### bin

The `bin` folder is for any system modules your package will use or generate.

* The compiled `node_gyp` output for your module's binary code.
* Pre-compiled platform binaries.
* [package.json/bin](https://docs.npmjs.com/files/package.json#bin) scripts for your module.

## How to organize GitHub Issues & Pull Requests

**Platform:**
- ![#bfd4f2](https://placehold.it/15/bfd4f2/000000?text=+) `angular`
- ![#bfd4f2](https://placehold.it/15/bfd4f2/000000?text=+) `bash`
- ![#bfd4f2](https://placehold.it/15/bfd4f2/000000?text=+) `browser`
- ![#bfd4f2](https://placehold.it/15/bfd4f2/000000?text=+) `ionic`
- ![#bfd4f2](https://placehold.it/15/bfd4f2/000000?text=+) `nodejs`
- ![#bfd4f2](https://placehold.it/15/bfd4f2/000000?text=+) `vue`

**Problems:**
- ![#ee3f46](https://placehold.it/15/ee3f46/000000?text=+) `bug`
- ![#ee3f46](https://placehold.it/15/ee3f46/000000?text=+) `security`

**Experience:**
- ![#ffc274](https://placehold.it/15/ffc274/000000?text=+) `ux`
- ![#ffc274](https://placehold.it/15/ffc274/000000?text=+) `ui`

**Environment:**
- ![#fad8c7](https://placehold.it/15/fad8c7/000000?text=+) `development`
- ![#fad8c7](https://placehold.it/15/fad8c7/000000?text=+) `production`
- ![#fad8c7](https://placehold.it/15/fad8c7/000000?text=+) `test`

**Feedback:**
- ![#cc317c](https://placehold.it/15/cc317c/000000?text=+) `discussion`
- ![#cc317c](https://placehold.it/15/cc317c/000000?text=+) `question`

**Improvements:**
- ![#5ebeff](https://placehold.it/15/5ebeff/000000?text=+) `enhancement`
- ![#5ebeff](https://placehold.it/15/5ebeff/000000?text=+) `optimization`
- ![#5ebeff](https://placehold.it/15/5ebeff/000000?text=+) `refactor`

**Additions:**
- ![#91ca55](https://placehold.it/15/91ca55/000000?text=+) `feature`

**Pending:**
- ![#fbca04](https://placehold.it/15/fbca04/000000?text=+) `backlog`
- ![#fbca04](https://placehold.it/15/fbca04/000000?text=+) `in progress`
- ![#fbca04](https://placehold.it/15/fbca04/000000?text=+) `on hold`

**Inactive:**
- ![#d2dae1](https://placehold.it/15/d2dae1/000000?text=+) `duplicate`
- ![#d2dae1](https://placehold.it/15/d2dae1/000000?text=+) `invalid`
- ![#d2dae1](https://placehold.it/15/d2dae1/000000?text=+) `wontfix`

**Miscellaneous:**
- ![#fef2c0](https://placehold.it/15/fef2c0/000000?text=+) `chore`
