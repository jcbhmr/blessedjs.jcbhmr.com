---
title: Blessed JavaScript
---

The JavaScript standard library doesn't cover everything. This "Blessed JavaScript" project curates the best solution for some common problems that fall outside the realm of the JavaScript standard library.

For a longer list of many other awesome JavaScript libraries, tools, and utilities check out [sindresorhus/awesome-nodejs](https://github.com/sindresorhus/awesome-nodejs) and [sorrycc/awesome-javascript](https://github.com/sorrycc/awesome-javascript).

## General

<table style="table-layout: fixed; width: 100%;">
<tr><th align=left>Random numbers<td>

[`crypto.getRandomValues()`](https://developer.mozilla.org/en-US/docs/Web/API/Crypto/getRandomValues)

<tr><th align=left>Time and date<td>

[Temporal API](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Temporal) via [temporal-polyfill](https://www.npmjs.com/package/temporal-polyfill)

<tr><th align=left>UUIDs<td>

[`crypto.randomUUID()`](https://developer.mozilla.org/en-US/docs/Web/API/Crypto/randomUUID) to generate v4 UUIDs.

[uuid](https://www.npmjs.com/package/uuid) for comprehensive generation and parsing.

<tr><th align=left>Temporary files<td>

[tempy](https://www.npmjs.com/package/tempy)

<tr><th align=left>Compression & decompression<td>

[Compression Streams API](https://developer.mozilla.org/en-US/docs/Web/API/Compression_Streams_API)

<tr><th align=left>HTTP requests<td>

[Fetch API](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API)

<tr><th align=left>Logging<td>

_TODO_

</table>

## Tooling

<table style="table-layout: fixed; width: 100%;">
<tr><th align=left>JavaScript runtimes<td>

[Node.js](https://nodejs.org/) is the most popular.

[Deno](https://deno.com/) and [Bun](https://bun.sh/) offer more comprehensive Node.js-compatible toolchains. See the [Deno](./deno/) and [Bun](./bun/) pages for more ecosystem-specific information.

<tr><th align=left>Toolchain management<td>

[nvm](https://github.com/nvm-sh/nvm) for Linux & macOS.

[nvm-windows](https://github.com/coreybutler/nvm-windows) for Windows.

<tr><th align=left>Code formatting<td>

[Biome](https://biomejs.dev/)

<tr><th align=left>Type checking<td>

[TypeScript](https://www.typescriptlang.org/)

<tr><th align=left>Linting<td>

[Biome](https://biomejs.dev/)

<tr><th align=left>Package managers<td>

[npm](https://www.npmjs.com/)

Use [pnpm](https://pnpm.io/) if you need its extra features.

<tr><th align=left>Testing<td>

[`node:test`](https://nodejs.org/api/test.html)

Use [Vitest](https://vitest.dev/) if you need its extra features.

</table>

## Math & science

<table style="table-layout: fixed; width: 100%;">
<tr><th align=left>Big decimal<td>

[js-big-decimal](https://www.npmjs.com/package/js-big-decimal)

</table>
