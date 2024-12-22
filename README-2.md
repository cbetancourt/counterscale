# Counterscale

⚠️ Last updated on 21-Dec-2024 with v2.3.0

This tracks the original instructions [found on the main repo](./README.md).

## Initial setup and deployment

1. Cloned the main repo
1. Deleted package lock and used PNPM
1. Run `pnpm dlx wrangler pages project create counterscale`
1. Run `pnpm dlx wrangler pages secret put CF_BEARER_TOKEN`
1. Run `pnpm dlx wrangler pages secret put CF_ACCOUNT_ID`
1. Run `pnpm build`
1. Run `pnpm dlx wrangler pages deploy ./build/client`

## Subsequent deployments

Update your site contents and run the last two commands again.

Each deployment results in a new FQDN, but the data already captured is not lost.
