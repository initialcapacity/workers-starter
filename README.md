# Cloudflare Workers Starter

https://starterapp.work

## Get started

1.  Run tests with NPM.
    ```shell
    npm test
    ```

1.  Create a `.dev.vars` file from the example.
    ```shell
    cp .dev.vars.example .dev.vars
    ```

1.  Edit the `.dev.vars` file to match your configuration.

1.  Migrate your local database.
    ```shell
    wrangler d1 migrations apply starter-db --local
    ```

1.  Run the scheduled worker.
    ```shell
    npm run worker:start
    ```

1.  Trigger the scheduled worker.
    ```shell
    npm run worker:trigger
    ```

1.  Run the auth app.
    ```shell
    npm run auth:start
    ```

1.  Run the app and visit [localhost:8788](http://localhost:8788).
    ```shell
    npm start
    ```

## Migrations

Run a migration with

```shell
wrangler d1 migrations create $MIGRATION_NAME
```
