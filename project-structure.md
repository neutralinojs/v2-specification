## Isolating static files directory

v1.x implementation

Since there is a pre-created `app/assets` directory, developers may try to put resources there while implementing an app by using a frontend library.

v2.x implementation 

Developers can specify the entry path via `entryPath` option in `neutralino.config.json`. Initially, `entryPath` directory will be served from the static file server.
Besides, when the developer is transpiling source files of the selected frontend framework, output files will be created inside `entryPath`.

## Adding a blank template

v1.x implementation

neu-cli doesn't provide a blank template. User typically needs to download manually from the releases.

v2.x implementation

`neu create test-app` or `neu create test-app --template blank` will create a minimal app with no frontend framework.

