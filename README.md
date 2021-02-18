# API Definition

API Definition repository

## Fast run

 * Install [Node JS](https://nodejs.org/).
 * Clone this repo and run `npm install` in the repo root.
 * Run `npm run api-doc`
 * Open the `./docs/index.html` in your favorite browser

## Generating the API Documentation with ReDoc

We used ReDoc CLI to generate the documentation from the API specification in our `.yml` file, so we installed `redoc-cli` like a development dependency in our project:

```
npm run redoc-blundle
```

ReDoc take the specification in our OpenAPI document and create an `index.html` file with the page with the documentation and place it into the `/docs` folder.

You can go to the `/docs` folder and open the `index.html` file in a browser and see how ReDoc has converted our plain specification in a great API documentation

## Automating the Documentation

We didn’t like to have to execute the command all times to see the changes in the API specification, so we configured our project to serve the documentation in a site and keeps the documentation updated while we modify the API definition in our specification file.

So, finally to make easy the documentation work you have to execute:

```
npm run api-doc
```

## Test the Specification

To test the specification we use the [OpenAPI CLI toolset](https://github.com/Redocly/openapi-cli) developed by the Redockly team.

To execute it, you only have to execute the following command:

```
npm run test
```

## Create the `dist` Folder

Execute:

```
npm run build
```

## Clean the Environment

Execute:

```
npm run clean
```

## Development

See the [CONTRIBUTING.md](./CONTRIBUTING.md) file

## License

See the [LICENSE](./LICENSE) file
