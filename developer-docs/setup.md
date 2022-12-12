# 🌳 Setup

## Pre-requisites

Before you follow the rest of this guide you'll want to make sure you have installed [Node.js](https://nodejs.org/) (>=16) and [pnpm](https://pnpm.io/). You'll also need Git setup to pull our source code from GitHub.

We also recommend using an IDE, such as [VSCode](https://code.visualstudio.com/), and the nx console plugin is recommended for creating dependencies.

## Installation

Clone our GitHub

```
git clone https://github.com/toeverything/AFFiNE.git
```

Currently we have two versions of AFFiNE:

* [AFFiNE Pre-Alpha](https://livedemo.affine.pro/). This version users the branch `master`, however is no longer actively developed and will be archived in the future.
* [AFFiNE Alpha](https://pathfinder.affine.pro/). This version uses the `pathfinder` branch, this is the latest version under active development. We plan to update this to the master branch in the near future.

Select the master branch

```
cd AFFiNE && git checkout pathfinder
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
