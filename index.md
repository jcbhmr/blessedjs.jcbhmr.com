---
title: Blessed JavaScript
---
<!--
NOTE: Custom CSS is in `_includes/head-custom.html` since the Markdown parser
that GitHub Pages uses doesn't like <style> tags in Markdown documents.
-->

# Blessed JavaScript

**Sometimes you need an npm package.** This list of "blessed" JavaScript npm packages (and other tools) helps you quickly find the best one for common use cases.

📚 Check out [sindresorhus/awesome-nodejs](https://github.com/sindresorhus/awesome-nodejs) and [sorrycc/awesome-javascript](https://github.com/sorrycc/awesome-javascript) for more comprehensive lists.

## General

<table>
<tr><th>Random numbers<td>

**`crypto.getRandomValues()`** [[docs]](https://developer.mozilla.org/en-US/docs/Web/API/Crypto/getRandomValues) \
Use to generate cryptographic random numbers. If you're not sure, use this.

**`Math.random()`** [[docs]](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math/random) \
Use to generate pseudo-random numbers

<tr><th>Time and date<td>

**Temporal API** [[docs]](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Temporal) \
The new comprehensive builtin time, date, and calendar API for JS. Not yet available in all environments.

**[temporal-polyfill](https://www.npmjs.com/package/temporal-polyfill)** [[docs]](https://github.com/fullcalendar/temporal-polyfill#readme) \
The best drop-in polyfill for the Temporal API. Use this until the native Temporal API is widely supported.

<tr><th>UUIDs<td>

**`crypto.randomUUID()`** [[docs]](https://developer.mozilla.org/en-US/docs/Web/API/Crypto/randomUUID) \
Use this builtin if you only need to generate v4 UUIDs

**[uuid](https://www.npmjs.com/package/uuid)** [[docs]](https://github.com/uuidjs/uuid#api) \
Use this if you need to generate more than just v4 UUIDs or do more than just generate UUIDs

<tr><th>Temporary files<td>

**[tempy](https://www.npmjs.com/package/tempy)** [[docs]](https://github.com/sindresorhus/tempy#api) \
Most popular temporary file & directory package for Node.js

<details><summary>See also</summary>

**`Deno.makeTempFile()`** [[docs]](https://docs.deno.com/examples/temporary_files/) \
Use the native Deno API instead of importing an npm package if you're using Deno

</details>

<tr><th>Compression & decompression<td>

**Compression Streams API** [[docs]](https://developer.mozilla.org/en-US/docs/Web/API/Compression_Streams_API) \
Use this builtin if it supports your format

**`node:zlib`** [[docs]](https://nodejs.org/api/zlib.html) \
Use this Node.js builtin if it supports your format as a second choice

<tr><th>Logging<td>

_TODO_

</table>

## Tooling

<table>
<tr><th>Desktop JavaScript runtimes<td>

**[Node.js](https://nodejs.org/)** [[docs]](https://nodejs.org/docs/latest/api/) \
The most popular desktop JavaScript runtime. If you're not sure, use this.

**[Deno](https://deno.com/)** [[docs]](https://docs.deno.com/) \
A comprehensive alternative JavaScript toolchain to Node.js & npm

**[Bun](https://bun.sh/)** [[docs]](https://bun.sh/docs) \
A faster Node.js & npm alternative with more features

<tr><th>Toolchain management<td>

**[nvm](https://github.com/nvm-sh/nvm)** [[docs]](https://github.com/nvm-sh/nvm#usage) \
Use this to manage Node.js versions for Linux & macOS. Officially recommended by https://nodejs.org/en/download.

**[fnm](https://github.com/Schniz/fnm)** [[docs]](https://github.com/Schniz/fnm#readme) \
Fast cross-platform Node.js manager. Officially recommended by https://nodejs.org/en/download.

<details><summary>See also</summary>

**`deno upgrade`** [[docs]](https://docs.deno.com/runtime/reference/cli/upgrade/) \
Prefer always using the latest Deno version

**`bun upgrade`** [[docs]](https://bun.sh/docs/installation#upgrading) \
Prefer always using the latest Bun version

</details>

<tr><th>Code formatting<td>

**[@biomejs/biome](https://www.npmjs.com/package/@biomejs/biome)** [[docs]](https://biomejs.dev/) \
The faster alternative to Prettier that also does linting. Use this in modern projects.

**[prettier](https://www.npmjs.com/package/prettier)** [[docs]](https://prettier.io/) \
The most popular JavaScript code formatter

<details><summary>See also</summary>

**`deno fmt`** [[docs]](https://docs.deno.com/runtime/reference/cli/fmt/) \
Use the builtin Deno formatter if you're using Deno

</details>

<tr><th>Type checking<td>

**[typescript](https://www.npmjs.com/package/typescript)** [[docs]](https://www.typescriptlang.org/) \
De-facto standard type checker for JavaScript

<details><summary>See also</summary>

**`deno check`** [[docs]](https://docs.deno.com/runtime/reference/cli/check/) \
Use Deno's TypeScript checking service if you're using Deno

</details>

<tr><th>Linting<td>

**[@biomejs/biome](https://www.npmjs.com/package/@biomejs/biome)** [[docs]](https://biomejs.dev/) \
The faster linter that also does formatting. Use this if you don't need custom plugins.

**[eslint](https://www.npmjs.com/package/eslint)** [[docs]](https://eslint.org/) \
The most popular JavaScript linter. Use this if you need to use plugins.

<details><summary>See also</summary>

**`deno lint`** [[docs]](https://docs.deno.com/runtime/fundamentals/linting_and_formatting/) \
Deno's builtin linter toolkit. Supports plugins. Use this if you're using Deno.

</details>

<tr><th>Package managers<td>

**[npm](https://www.npmjs.com/)** [[docs]](https://docs.npmjs.com/) \
The bundled package manager that comes with Node.js. Use this if you're undecided.

**[pnpm](https://pnpm.io/)** [[docs]](https://pnpm.io/motivation) \
Use this if you need its extra features like dependency patching

<details><summary>See also</summary>

**`deno add`** [[docs]](https://deno.com/blog/your-new-js-package-manager) \
Use the Deno package manager if you're using Deno

**`bun pm`** [[docs]](https://bun.sh/docs/cli/pm) \
Use the Bun package manager if you're using Bun

</details>

<tr><th>Testing<td>

**`node:test`** [[docs]](https://nodejs.org/api/test.html) \
The included Node.js test toolkit. Use this if possible. May use `node:assert` for assertions. Also works with Deno and Bun.

**[vitest](https://www.npmjs.com/package/vitest)** [[docs]](https://vitest.dev/) \
Vite's accompanying testing tool. Use this if you're using Vite or need its extra features like browser testing.

<details><summary>See also</summary>

**`Deno.test()`** [[docs]](https://docs.deno.com/runtime/fundamentals/testing/) \
Deno's builtin testing toolkit. Use this if you're using only Deno.

**`bun:test`** [[docs]](https://bun.sh/docs/cli/test) \
Bun's builtin testing toolkit. Use this if you're using only Bun.

</details>

</table>

## Schema & validation

<table>
<tr><th>JSON schema<td>

**[ajv](https://ajv.js.org/)** [[docs]](https://ajv.js.org/guide/getting-started.html) \
The most popular JSON schema validation library.

</table>

## Math & science

<table>
<tr><th>Big decimal<td>

TODO

<tr><th>Linear algebra<td>

TODO

<tr><th>DataFrames<td>

TODO

</table>

## FFI & interop

<table>
<tr><th>C/C++ to JS<td>

**[ffi-rs](https://www.npmjs.com/package/ffi-rs)** [[docs]](https://github.com/zhangyuang/node-ffi-rs#readme) \
Runtime `dlopen()` with types for Node.js and friends. Use this on existing `.so`/`.dylib`/`.dll` dynamic libraries.

<tr><th>Rust to JS<td>

**[napi-rs](https://www.npmjs.com/package/@napi-rs/cli)** [[docs]](https://napi.rs/) \
Use `#[napi]` annotations to expose Rust functions to JavaScript via the C Node-API.

**[wasm-bindgen](https://docs.rs/wasm-bindgen/latest/wasm_bindgen/)** [[docs]](https://rustwasm.github.io/wasm-bindgen/) \
Use `#[wasm_bindgen]` annotations to expose Rust functions to JavaScript via WebAssembly

</table>

## Networking

<table>
<tr><th>HTTP client<td>

**Fetch API** [[docs]](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API) \
Node.js has `fetch()` builtin now. Use it.

<tr><th>HTTP server<td>

**[hono](https://www.npmjs.com/package/hono)** [[docs]](https://hono.dev/) \
Rising standards-based web server framework

**[express](https://www.npmjs.com/package/express)** [[docs]](https://expressjs.com/) \
The most popular Node.js HTTP framework

<tr><th>WebSocket client<td>

**`WebSocket`** [[docs]](https://developer.mozilla.org/en-US/docs/Web/API/WebSocket) \
Basic WebSocket client available in Node.js & friends and browsers. Single event stream. Use this for basic tasks.

**[socket.io](https://www.npmjs.com/package/socket.io)** [[docs]](https://socket.io/) \
Comprehensive popular WebSocket wrapper for servers and clients. Supports multiplexing. Use this if your server uses socket.io.

<tr><th>WebSocket server<td>

**[socket.io](https://www.npmjs.com/package/socket.io)** [[docs]](https://socket.io/) \
Comprehensive popular WebSocket wrapper for servers and clients. Supports multiplexing.

</table>

## CLIs

<table>
<tr><th>Argument parsing<td>

**`util.parseArgs()`** [[docs]](https://nodejs.org/api/util.html#utilparseargsconfig) \
Basic builtin argument parsing. Use this for local project scripts.

TODO

<tr><th>Globbing<td>

**`fs.promises.glob()`** [[docs]](https://nodejs.org/api/fs.html#fspromisesglobpattern-options) \
Node.js now has builtin globbing support. Use this unless you need more features.

**[globby](https://www.npmjs.com/package/globby)** [[docs]](https://github.com/sindresorhus/globby#api) \
Globber that deals with `.gitignore` too.

<tr><th>File watching<td>

**[watcher](https://www.npmjs.com/package/watcher)** [[docs]](https://github.com/fabiospampinato/watcher#usage) \
The most complete file & directory watcher.

</table>
