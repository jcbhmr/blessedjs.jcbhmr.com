# Recommended npm package directory

- TOC
{:toc}

## General

Random numbers
: [`crypto.getRandomValues()`](https://developer.mozilla.org/en-US/docs/Web/API/Crypto/getRandomValues): Fills a `TypedArray` with random data. Available in Node.js & browsers.

Time and date
: [temporal-polyfill](https://www.npmjs.com/package/temporal-polyfill): Use a Temporal API polyfill until the Temporal API is widely supported.
: [Temporal API](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Temporal): Use the native Temporal API without a polyfill when possible.

UUIDs
: [`crypto.randomUUID()`](https://developer.mozilla.org/en-US/docs/Web/API/Crypto/randomUUID): Generates a v4 UUID. Available in Node.js & browsers.
: [uuid](https://www.npmjs.com/package/uuid): A full-featured comprehensive UUID API.

Temporary files
: [tempy](https://www.npmjs.com/package/tempy): Use a callback to automatically create & delete a temporary file after use.

Gzip compression & decompression
: [Compression Streams API](https://developer.mozilla.org/en-US/docs/Web/API/Compression_Streams_API): Compress & decompress using the Streams API. Available in Node.js & browsers.

HTTP requests
: [Fetch API](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API): Available in Node.js & browsers.

Text-based logging
: _Unknown_

Structured logging
: _Unknown_

Runtimes
: [Node.js](https://nodejs.org/): Most popular desktop JavaScript runtime.
: [Deno](https://deno.com/): AiO JS/TS runtime, package manager, linter, formatter, and more.
: [Bun](https://bun.sh/): Faster AiO Node.js & npm drop-in replacement.

Toolchain management
: _Lots_

Code formatting
: [Biome](https://biomejs.dev/): Faster streamlined Prettier & ESLint replacement.

Linting
: [TypeScript](https://www.typescriptlang.org/)
: [Biome](https://biomejs.dev/): Faster streamlined Prettier & ESLint replacement.
: [Deno](https://deno.com/): AiO JS/TS runtime, package manager, linter, formatter, and more.

Package managers
: [npm](https://www.npmjs.com/): The default standard Node.js package manager. Use this with Node.js.
: [pnpm](https://pnpm.io/): npm but faster and with more features. Use this with Node.js if you need to patch a dependency.
: [Deno](https://deno.com/): AiO JS/TS runtime, package manager, linter, formatter, and more.
: [Bun](https://bun.sh/): Faster AiO Node.js & npm drop-in replacement.

Testing
: [`node:test`](https://nodejs.org/api/test.html): Node.js/Deno/Bun basic test runner.
: [Vitest](https://vitest.dev/): AiO JS/TS testing toolkit built on Vite. Supports browser testing too.

Benchmarking
: [Vitest](https://vitest.dev/): AiO JS/TS testing toolkit built on Vite. Supports browser testing too.
