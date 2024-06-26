# Typesafe REST API Specification - Library Aggregator Packages

[![CI Pipeline](https://github.com/devtea2028/reimagined-octo-fortnight/actions/workflows/ci.yml/badge.svg)](https://github.com/devtea2028/reimagined-octo-fortnight/actions/workflows/ci.yml)
[![CD Pipeline](https://github.com/devtea2028/reimagined-octo-fortnight/actions/workflows/cd.yml/badge.svg)](https://github.com/devtea2028/reimagined-octo-fortnight/actions/workflows/cd.yml)

The Typesafe REST API Specification is a family of libraries used to enable seamless development of Backend and/or Frontend which communicate via HTTP protocol.
The protocol specification is checked both at compile-time and run-time to verify that communication indeed adhers to the protocol.
This all is done in such way that it does not make development tedious or boring, but instead robust and fun!

This particular repository contains libraries, which act as aggregators for a set of other libraries.
The purpose is to make life of users easier, which will only need to write one
```ts
import * as tyras from "@ty-ras/backend-node-io-ts-openapi";
```
instead of many
```ts
import * as tyrasData from "@ty-ras/data";
import * as tyrasDataBE from "@ty-ras/data-backend";
...etc
```

# Data validation using `io-ts`
This repository contains the following aggregator libraries for [`io-ts`](https://github.com/gcanti/io-ts) framework:
- [`@ty-ras/backend-node-io-ts-openapi`](./code/backend-node-io-ts-openapi) for backends using Node HTTP(S) 1/2 server, `io-ts` as data validation library, and OpenAPI as metadata format,
- [`@ty-ras/backend-koa-io-ts-openapi`](./code/backend-koa-io-ts-openapi) for backends using Koa HTTP(S) 1/2 server, `io-ts` as data validation library, and OpenAPI as metadata format,
- [`@ty-ras/backend-express-io-ts-openapi`](./code/backend-express-io-ts-openapi) for backends using Express HTTP(S) 1 server, `io-ts` as data validation library, and OpenAPI as metadata format,
- [`@ty-ras/backend-fastify-io-ts-openapi`](./code/backend-fastify-io-ts-openapi) for backends using Fastify HTTP(S) 1/2 server, `io-ts` as data validation library, and OpenAPI as metadata format,
- [`@ty-ras/frontend-fetch-io-ts`](./code/frontend-fetch-io-ts) for frontend clients using Fetch API to send HTTP requests and `io-ts` as data validation library,
- [`@ty-ras/frontend-node-io-ts`](./code/frontend-node-io-ts) for frontend clients using Node runtime to send HTTP requests and `io-ts` as data validation library,
- [`@ty-ras/frontend-axios-io-ts`](./code/frontend-axios-io-ts) for frontend clients using [Axios](https://github.com/axios/axios) library to send HTTP requests and `io-ts` as data validation library,
- [`@ty-ras-extras/backend-io-ts`](./code/extras-backend-io-ts) for most typically used extra functionality (caching, configuration, resource pool, main invocation, SQL) in backend, and
- [`@ty-ras-extras/frontend-io-ts`](./code/extras-frontend-io-ts) for most typically used extra functionality (caching, configuration) in frontend.

# Data validation using `zod`
This repository contains the following aggregator libraries for [`zod`](https://github.com/colinhacks/zod) framework:
- [`@ty-ras/backend-node-zod-openapi`](./code/backend-node-zod-openapi) for backends using Node HTTP(S) 1/2 server, `zod` as data validation library, and OpenAPI as metadata format,
- [`@ty-ras/backend-koa-io-ts-openapi`](./code/backend-koa-io-ts-openapi) for backends using Koa HTTP(S) 1/2 server, `zod` as data validation library, and OpenAPI as metadata format,
- [`@ty-ras/backend-express-io-ts-openapi`](./code/backend-express-io-ts-openapi) for backends using Express HTTP(S) 1 server, `zod` as data validation library, and OpenAPI as metadata format,
- [`@ty-ras/backend-fastify-io-ts-openapi`](./code/backend-fastify-io-ts-openapi) for backends using Fastify HTTP(S) 1/2 server, `zod` as data validation library, and OpenAPI as metadata format,
- [`@ty-ras/frontend-fetch-zod`](./code/frontend-fetch-zod) for frontend clients using Fetch API to send HTTP requests and `zod` as data validation library,
- [`@ty-ras/frontend-node-zod`](./code/frontend-node-zod) for frontend clients using Node runtime to send HTTP requests and `zod` as data validation library,
- [`@ty-ras/frontend-axios-zod`](./code/frontend-axios-zod) for frontend clients using [Axios](https://github.com/axios/axios) library to send HTTP requests and `zod` as data validation library,
- [`@ty-ras-extras/backend-zod`](./code/extras-backend-zod) for most typically used extra functionality (caching, configuration, resource pool, main invocation, SQL) in backend, and
- [`@ty-ras-extras/frontend-zod`](./code/extras-frontend-zod) for most typically used extra functionality (caching, configuration) in frontend.

# Data validation using `runtypes`
This repository contains the following aggregator libraries for [`runtypes`](https://github.com/pelotom/runtypes) framework:
- [`@ty-ras/backend-node-runtypes-openapi`](./code/backend-node-runtypes-openapi) for backends using Node HTTP(S) 1/2 server, `runtypes` as data validation library, and OpenAPI as metadata format,
- [`@ty-ras/backend-koa-io-ts-openapi`](./code/backend-koa-io-ts-openapi) for backends using Koa HTTP(S) 1/2 server, `runtype` as data validation library, and OpenAPI as metadata format,
- [`@ty-ras/backend-express-io-ts-openapi`](./code/backend-express-io-ts-openapi) for backends using Express HTTP(S) 1 server, `runtype` as data validation library, and OpenAPI as metadata format,
- [`@ty-ras/backend-fastify-io-ts-openapi`](./code/backend-fastify-io-ts-openapi) for backends using Fastify HTTP(S) 1/ server, `runtype` as data validation library, and OpenAPI as metadata format,
- [`@ty-ras/frontend-fetch-runtypes`](./code/frontend-fetch-runtypes) for frontend clients using Fetch API to send HTTP requests and `runtypes` as data validation library,
- [`@ty-ras/frontend-node-runtypes`](./code/frontend-node-runtypes) for frontend clients using Node runtime to send HTTP requests and `runtypes` as data validation library,
- [`@ty-ras/frontend-axios-runtypes`](./code/frontend-axios-runtypes) for frontend clients using [Axios](https://github.com/axios/axios) library to send HTTP requests and `runtypes` as data validation library,
- [`@ty-ras-extras/backend-runtypes`](./code/extras-backend-runtypes) for most typically used extra functionality (caching, configuration, resource pool, main invocation, SQL) in backend, and
- [`@ty-ras-extras/frontend-runtypes`](./code/extras-frontend-zod) for most typically used extra functionality (caching, configuration) in frontend.
