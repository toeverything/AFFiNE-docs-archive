# Deploy AFFINE to Vercel
[Vercel](https://vercel.com) is the platform for frontend developers, providing the speed and reliability innovators need to create at the moment of inspiration.

`AFFINE` can be simply deployed to `Vercel` with just a few mouse clicks because `Vercel` fully supports `Nextjs`, which is the stack used by `AFFINE`.

Before we begin, we'll assume you already have a `Vercel` account and have connected it to your `Github` account.

1. Fork [AFFINE](https://github.com/toeverything/AFFiNE) to your onn `Github` account.
1. After logging in to [Vercel](https://vercel.com), go to your hobby page and click the `Add New... - Project` button.
1. Click the `Import` button after selecting the AFFINE repository you forked (if you cannot access your repository, go to the Vercel team's [guide](https://vercel.com/docs/concepts/git#deploying-a-git-repository)).
1. Next, configure your project as follows:
   <img src="../.gitbook/assets/getting-started_deploy-affine-to-vercel_config-project.png" alt="config project">
   - Build Command - `AFFINE` use pnpm to build whole app
   - Output Directory - output of build assets in app folder
   - Install Command - since we set up `AFFINE` as a `Nextjs` project, `Vercel` will detect `Nextjs` dependencies, but our work dir is root dir, if we do not hoist dependencies to top level, `Vercel` cannot find `Nextjs` dependencies, there are some error occurred
1. To deploy `AFFINE` to a production environment, click `Deploy`.
1. After building is complete, go to the address that `Vercel` provided and enjoy!

## Troubleshooting
If your building fails, go to the project settings page and verify whether your `Root Directory` is accurate.

Not sure if this is an issue with Vercel, but sometimes building failed when I set the `Root Directory` to `./` during the initialization of the project.

<img src="../.gitbook/assets/getting-started_deploy-affine-to-vercel_set-root-directory.png" alt="set root directory">

You can simply leave it empty or set it up using `./` as suggested in the tips.
