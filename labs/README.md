## Pre-Lab Setup

1. `cd` into the repo root.
2. Start the container.
   - Run `npm start`
3. Get the `Root Token`
   - Run `docker logs vault_vault_1 | grep "Root Token"` to see the logs, and then look for `Root Token`.
4. Shell into the container.
   - Run `docker exec -it vault_vault_1 bash`
5. Set the `VAULT_TOKEN` env var to the `Root Token`.
   - Run `export VAULT_TOKEN=<root_token>`
     - Where `<root_token>` is the `Root Token.

## Post-Lab Teardown

1. Run `npm stop`
