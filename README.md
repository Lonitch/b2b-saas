# SaaS project with BETH stack
- Create BETH app with [this](https://www.npmjs.com/package/create-beth-app) and the command `install create-beth-app@0.0.6`
- open an issue [here](https://github.com/ethanniser/the-beth-stack)
- forum [here](https://discord.gg/Z3yUtMfkwa)

## To run locally:

1. `bun install`
2. create a new turso database with `turso db create <name>`
3. get the database url with `turso db show --url <name>`
4. get the auth token with `turso db tokens create <name>`
5. (optional) create a new github developer app and get credentials
6. copy `.env.example` to `.env`
7. fill out all enviorment variables (refer to the config file to see schema)
8. `bun db:push`
9. `bun dev`

## To deploy to fly.io

1. Install the [Fly CLI](https://fly.io/docs/hands-on/install-flyctl/)

2. Run `fly launch`

3. Run `fly secrets set <NAME>=<VALUE>` (probably want to set `NODE_ENV` to `"production"`)

5. Run `fly deploy`

## DevOps
repo: `git remote add origin https://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@github.com/Lonitch/b2b-saas.git`