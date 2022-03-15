## Introduction

This is a fork of [prism](https://github.com/stoplightio/prism).

## Setup

```
yarn build --clean
```

build docker image

```
cd ${rootPath}
docker image -t <image-name> .
```

start image

```
docker run --init -p 4010:4010 openprism:demo mock -h 0.0.0.0 /tmp/specification/storage/resource-manager/Microsoft.Storage/stable/2021-08-01/storage.json
```

or

```
docker run --init -p 4010:4010 openprism:demo mock -h 0.0.0.0 https://raw.githubusercontent.com/1openwindow/openprism/master/examples/petstore.oas2.yaml
```

in dev env, you may need to set the following parameter in env.

```
NODE_TLS_REJECT_UNAUTHORIZED = 0
```

## 🎉 Thanks

Prism is built on top of lots of excellent packages, and here are a few we'd like to say a special thanks to.

- [prism](https://github.com/stoplightio/prism)
- [ajv](https://www.npmjs.com/package/ajv)
- [faker](https://www.npmjs.com/package/faker)
- [fp-ts](https://www.npmjs.com/package/fp-ts)
- [gavel](https://www.npmjs.com/package/gavel)
- [json-schema-faker](https://www.npmjs.com/package/json-schema-faker)
- [lerna](https://www.npmjs.com/package/lerna)
- [micri](https://www.npmjs.com/package/micri)
- [openapi-sampler](https://www.npmjs.com/package/openapi-sampler)
- [yargs](https://www.npmjs.com/package/yargs)
