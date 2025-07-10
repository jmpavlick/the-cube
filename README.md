# README

Summon `THE CUBE`.

Tech demo:

- `elm-pages` deployed on Vercel with Vercel Serverless function execution
- AR demo of possible new "storage unit calculator" (requires iOS at the moment, sorry, but this is not a permanent condition)
- Uses `direnv` + `vercel` (CLI) to synchronize environment variables
- Demonstrates reading environment variables on production at build time through an `elm-pages` `BackendTask`
- CI/CD is all automatic, Vercel gives us preview branching immediately on pull-request