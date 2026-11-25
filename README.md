# ice-cream-dataops
Cognite Data Fusion Bootcamp

The GitHub Actions deployment defaults to the `dev` environment and targets
`sudheeriv-dev`. Opening, reopening, or updating a pull request from a branch in
this repository automatically deploys to dev. Pull requests from forks are
skipped because deployment credentials are not available to untrusted forks.

Configure the GitHub `dev` environment with these variables:
`IDP_TENANT_ID`, `IDP_TOKEN_URL`, `IDP_SCOPES`, `IDP_CLIENT_ID`,
`DATA_DEVELOPER_SOURCE_ID`, `DATA_PIPELINE_OEE_CLIENT_ID`,
`DATA_PIPELINE_OEE_SOURCE_ID`, `ICAPI_EXTRACTORS_CLIENT_ID`, and
`ICAPI_EXTRACTORS_SOURCE_ID`. Add `IDP_CLIENT_SECRET`,
`DATA_PIPELINE_OEE_CLIENT_SECRET`, and `ICAPI_EXTRACTORS_CLIENT_SECRET` as
GitHub environment secrets. Use the values from the local dev configuration;
do not commit the `.env` file.

Manual workflow runs can still select `prod`.
