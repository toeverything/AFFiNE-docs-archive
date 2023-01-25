# 🌳 Setup

## Pre-requisites

Before you follow the rest of this guide you'll want to make sure you have installed [Node.js](https://nodejs.org/) (>=16) and [pnpm](https://pnpm.io/) (>7.x). You'll also need Git setup to pull our source code from GitHub.

We also recommend using an IDE, such as [VSCode](https://code.visualstudio.com/), and the nx console plugin is recommended for creating dependencies.

## Installation

Clone our GitHub

```
git clone https://github.com/toeverything/AFFiNE.git
```

Currently we have two versions of AFFiNE:

* [AFFiNE Alpha](https://pathfinder.affine.pro/). This version uses the `master` branch, this is the latest version under active development. We plan to update this to the master branch in the near future.
* [AFFiNE Pre-Alpha](https://livedemo.affine.pro/). This version uses the branch `pre-alpha`, however is no longer actively developed and has been effectively archived.

Select the master branch

```
cd AFFiNE
```

Install dependencies

```
pnpm install
```

Start AFFiNE

```
pnpm dev
```

Default settings will run AFFiNE on localhost, port 3000 - http://localhost:3000

## Further Steps

The `.env.local` file can be found in the project folder. You can add the following variable to enable the development environment.

```
NODE_ENV=development
```

For git-cz functionality, please install the corresponding dependencies globally.

```
npm install -g commitizen conventional-changelog conventional-changelog-cli
```
