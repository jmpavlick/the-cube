# `THE CUBE`

Summon `THE CUBE`.

Tech demo:

- `elm-pages` deployed on Vercel with Vercel Serverless function execution
- AR demo of possible new "storage unit calculator" (requires iOS at the moment, sorry, but this is not a permanent condition)
- Uses `direnv` + `vercel` (CLI) to synchronize environment variables
- Demonstrates reading environment variables on production at build time through an `elm-pages` `BackendTask`
- CI/CD is all automatic, Vercel gives us preview branching immediately on pull-request

# Setup

- Install `pnpm`: `npm i -g pnpm` (it's better)
- Install `direnv`:
  - `brew install direnv`
  - Add `eval "$(direnv hook bash)"` to your `~/.bash_profile` or whatever
- You might need to run `vercel login` to pull env vars:
  - `pnpx vercel login`, and `pnpx vercel link` to project `the-cube`
  - If you don't have a Vercel login, add the missing env var to `.env` manually:
    - `OPTIONAL_VERCEL_SERVERLESS_FN_OVERRIDE_URL=http://localhost:3000`

# Running

- `pnpm vdev`
