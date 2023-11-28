# Showcasing ref resolving in Redocly CLI 
## Preparation
Make sure you have the [redocly cli](https://redocly.com/docs/cli/installation/) installed.
## Run demonstration
[openapi.yaml](openapi.yaml) contains a OpenAPI spec that references a schema in [schemas.yaml](schemas.yaml).
One can bundle the spec and the schema into a single file by executing: 
```bash
redocly bundle openapi.yaml -o bundled.yaml
```
The [bundled.yaml](bundled.yaml) will contain the referenced schema in the components section of the OpenAPI spec so that
tools can still use the original schema name.