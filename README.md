# action-central

Simple template with basic Amplify Central action. On push, any yaml resources in this repo will be applied to Amplify Central.

> *Note:* Currently this is very simple. On push it finds all the yamls and merges them into a single file. This is then applied by the CLI. It sorts our ordering and change. This has the side effect of making deletion undetectable.

# Secrets

| Secret       | Description  |
|--------------|--------------|
| ENVIRONMENT  | The environment to use [prod\|prepod]. |
| CLIENT_ID    | The service account client id.  |
| PRIVATE_KEY  | The service account private key (PEM format). |
| BASE_URL     | The Amplify Central url (http://apicentral.axway.com). Note no trailing slash - if you add one you'll see "Cannot read property 'resourceVersion' of undefined". |

