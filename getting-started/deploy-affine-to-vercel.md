# Deploy AFFiNE to Vercel
[Vercel](https://vercel.com) is a platform for frontend developers, providing the speed and reliability innovators need to create at the moment of inspiration.

`AFFiNE` can be simply deployed to `Vercel` with just a few mouse clicks because `Vercel` fully supports `Next.js`, which is the stack used by `AFFiNE`.

Before we begin, we'll assume you already have a `Vercel` account and have connected it to your `GitHub` account.

1. Fork [AFFiNE](https://github.com/toeverything/AFFiNE) to your own `GitHub` account.
1. After logging in to [Vercel](https://vercel.com), go to your hobby page and click the `Add New... - Project` button.
1. Click the `Import` button after selecting the AFFINE repository you forked (if you cannot access your repository, go to the Vercel team's [guide](https://vercel.com/docs/concepts/git#deploying-a-git-repository)).
1. Next, configure your project as follows:
    - Build Command - `AFFiNE` uses pnpm to build whole app
    - Output Directory - output of build assets in the app folder
    - Install Command - since we set up `AFFiNE` as a `Next.js` project, `Vercel` will detect `Next.js` dependencies, but the work dir is the root dir, so this is required as `Vercel` will otherwise not find `Next.js` dependencies
    <figure>
        <img width="967" alt="image" src="https://github.com/toeverything/AFFiNE-docs/assets/5910926/ad9599c0-5a35-47d3-8f91-9eb431120c10">
<figcaption></figcaption></figure>
1. To deploy `AFFiNE` to a production environment, click `Deploy`.
1. After building is complete, go to the address that `Vercel` provides and enjoy!

## Troubleshooting
If your building fails, go to the project settings page and verify whether your `Root Directory` is accurate.

Sometimes building fails when the `Root Directory` is set to `./` during the initialization of the project.

<figure><img width="967" alt="image" src="https://github.com/toeverything/AFFiNE-docs/assets/5910926/ea78d3fb-f042-4150-8b51-6f2448f95df4">
<figcaption></figcaption></figure>

You can simply leave it empty or set it up using `./` as suggested in the tips.
