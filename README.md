# PostHog.js

Please see the main [PostHog docs](https://posthog.com/docs).

Specifically, the [JS integration](https://posthog.com/docs/integrations/js-integration) details.

## Testing

Run `yarn test`

## Releasing a new version

To release a new version, make sure you're logged in to NPM (`npm login`)

We tend to follow the following steps:

1. Merge your changes into master
2. Release changes as a beta version
    - `npm version 1.x.x-beta.0`
    - `npm publish --tag beta`
3. Create a PR linking to this version [in the main repo](https://github.com/posthog/posthog)
4. Once deployed and tested, write up CHANGELOG.md, and commit.
5. Release a new version
    - `npm version 1.x.x`
    - `npm publish`
6. Create a PR linking to this version [in the main repo](https://github.com/posthog/posthog)
