# 🌳 Quick Start

## Installation

To setup the AFFiNE development environment, please make sure you have installed [Node.js](https://nodejs.org/) (>=16) and [pnpm](https://pnpm.io/).

```shell
# Clone the repo and make sure using right branch
git clone https://github.com/toeverything/AFFiNE.git
cd AFFiNE && git checkout master

# Install dependencies
pnpm install
```

Then AFFiNE is ready to start.

```shell
# Start the project
pnpm start
open http://localhost:4200/
```

For using development environment, the following [environment variable](https://en.wikipedia.org/wiki/Environment\_variable#Assignment:\_Unix) config can be copied into the `.env.local` file in project root.

```shell
NODE_ENV=development
```

For `git-cz` functionalities, please install corresponding dependencies globally.

```
npm install -g commitizen conventional-changelog conventional-changelog-cli
```

## Quick Overview

The basic directory structure conventions in this repository are described here.

* Generic functional components (e.g., atomic UI components) are placed in `libs/components/common.`
  * Components within `common` are not allowed to import other _components_ except utils and dependencies.
  * Common components can dependent on each other.
* Components containing business logic are placed in `libs/components`. The `editor` and `draw` prefixes are used to distinguish them.
* The data source components are placed in `libs/datasource`, including API requests, schemas, etc.

Please checkout the `docs/CONTRIBUTING` documentation for more details.

## Useful Scripts

Some commonly used commands defined in `package.json` are listed here.

```shell
# Create react dependency library
pnpm run add:library

# Create react components
pnpm run add:components

# Create a data source
pnpm run add:datasource

# Run unit tests
pnpm test

# Compile or test or lint specific component
pnpm build|test|lint ${project name from workspace.json}
```

## IDE Support

We recommend developing AFFiNE with [VSCode](https://code.visualstudio.com/), and the [nx console](https://marketplace.visualstudio.com/items?itemName=nrwl.angular-console) plugin is also recommended for creating dependencies.
