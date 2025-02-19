The JavaScript standard library doesn't cover everything. This "Blessed JavaScript" project curates the best solution for some common problems that fall outside the realm of the JavaScript standard library.

#### Random numbers

Use [`crypto.getRandomValues()`](https://developer.mozilla.org/en-US/docs/Web/API/Crypto/getRandomValues). It's available in Node.js, Deno, Bun, and browsers.

#### Time and date

Use the [Temporal API](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Temporal) if you can. Right now it doesn't have universal support so you'll need a polyfill like [temporal-polyfill](https://www.npmjs.com/package/temporal-polyfill).

#### UUIDs

If you only need to generate v4 UUIDs then use [`crypto.randomUUID()`](https://developer.mozilla.org/en-US/docs/Web/API/Crypto/randomUUID). It's available in Node.js, Deno, Bun, and browsers. If you need something more comprehensive then use [uuid](https://www.npmjs.com/package/uuid).

#### Temporary files

Use [tempy](https://www.npmjs.com/package/tempy).

#### Compression & decompression

Use the [Compression Streams API](https://developer.mozilla.org/en-US/docs/Web/API/Compression_Streams_API). It's available in Node.js, Deno, Bun, and browsers.

#### HTTP requests

Use the [Fetch API](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API). There's no need to use node-fetch anymore; Node.js, Deno, Bun, and browsers all universally support fetch.

#### Logging

TODO

#### JavaScript runtimes

The most popular desktop JavaScript runtime is [Node.js](https://nodejs.org/). [Deno](https://deno.com/) and [Bun](https://bun.sh/) offer more comprehensive Node.js-compatible toolchains if you prefer a more all-in-one toolkit than Node.js provides.

#### Toolchain version management

The most popular Node.js version manager is [nvm](https://github.com/nvm-sh/nvm) for Linux & macOS. [nvm-windows](https://github.com/coreybutler/nvm-windows) is a similar popular project for Windows users.

#### Code formatting

Use [Biome](https://biomejs.dev/) which is like [Prettier](https://prettier.io/) but faster.

If you're using Deno it comes with its own [`deno fmt`](https://docs.deno.com/runtime/reference/cli/fmt/).

#### Type checking

Use [TypeScript](https://www.typescriptlang.org/).

If you're using Deno it comes with its own [`deno check`](https://docs.deno.com/runtime/reference/cli/check/).

#### Linting

Prefer zero-config [Biome](https://biomejs.dev/). If you need to write custom rules, use [ESLint](https://eslint.org/).

If you're using Deno it comes with its own [`deno lint`](https://docs.deno.com/runtime/reference/cli/lint/).

#### Package managers

Use the default [npm](https://www.npmjs.com/) unless you need [pnpm](https://pnpm.io/)'s extra features.

If you're using Deno it comes with its own [`deno add` and friends](https://deno.com/blog/your-new-js-package-manager).

If you're using Bun it comes with its own [`bun pm`](https://bun.sh/docs/cli/pm).

#### Testing

Use [`node:test`](https://nodejs.org/api/test.html) and `node --test`. It works with Node.js, Deno, and Bun. Use [Vitest](https://vitest.dev/) if you need more mocking features. Vitest also lets you write [Playwright](https://playwright.dev/) tests.

If you're using Deno it comes with its own [`deno test` toolset](https://docs.deno.com/runtime/fundamentals/testing/).

If you're using Bun it comes with its own [`bun test` toolset](https://bun.sh/docs/cli/test).

#### Benchmarking

Use [Vitest](https://vitest.dev/).

If you're using Deno it comes with its own [`deno bench` toolset](https://docs.deno.com/runtime/fundamentals/testing/).

#### Big decimal

Use [js-big-decimal](https://www.npmjs.com/package/js-big-decimal).
