- **Random numbers:** [`crypto.getRandomValues()`](https://developer.mozilla.org/en-US/docs/Web/API/Crypto/getRandomValues)
- **Time and date:**
  - **Forward thinking:** [Temporal API](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Temporal) via [temporal-polyfill](https://www.npmjs.com/package/temporal-polyfill)
  - **Interop with `Date`:** [date-fns](https://date-fns.org/)
  - **Instead of `Date`:** [dayjs](https://day.js.org/)
- **UUIDs:**
  - **Generate v4 only:** [`crypto.randomUUID()`](https://developer.mozilla.org/en-US/docs/Web/API/Crypto/randomUUID)
  - **Comprehensive:** [uuid](https://www.npmjs.com/package/uuid)
- **Temporary files**: [tempy](https://www.npmjs.com/package/tempy)
- **Gzip compression & decompression:** [Compression Streams API](https://developer.mozilla.org/en-US/docs/Web/API/Compression_Streams_API)
- **HTTP requests:** [Fetch API](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API)
- **Logging:** _TODO_
- **JavaScript runtimes:**
  - **Most popular:** [Node.js](https://nodejs.org/)
  - **Most comprehensive:** [Deno](https://deno.com/)
  - **Most performant:** [Bun](https://bun.sh/)
- **Toolchain management:** _TODO_
- **Code formatting:**
  - **Fastest:** [Biome](https://biomejs.dev/)
  - **Most popular:** [Prettier](https://prettier.io/)
- **Type checking:** [TypeScript](https://www.typescriptlang.org/)
- **Linting:**
  - **Fastest:** [Biome](https://biomejs.dev/)
  - **Most customizable:** [ESLint](https://eslint.org/)
  - **Deno:** [`deno lint`](https://docs.deno.com/runtime/reference/cli/lint/)
- **Package managers:**
  - **Node.js:** [npm](https://www.npmjs.com/)
  - **Deno:** [`deno add` and friends](https://deno.com/blog/your-new-js-package-manager)
  - **Bun:** [`bun pm`](https://bun.sh/docs/cli/pm)

<!--
Testing
: [`node:test`](https://nodejs.org/api/test.html): Node.js/Deno/Bun basic test runner.
: [Vitest](https://vitest.dev/): AiO JS/TS testing toolkit built on Vite. Supports browser testing too.

Benchmarking
: [Vitest](https://vitest.dev/): AiO JS/TS testing toolkit built on Vite. Supports browser testing too.
-->
