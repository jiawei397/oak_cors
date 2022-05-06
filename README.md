# oak_cors

[![Deno](https://github.com/jiawei397/oak_cors/actions/workflows/deno.yml/badge.svg)](https://github.com/jiawei397/oak_cors/actions/workflows/deno.yml)

Forked from the nodejs package
[expressjs cors](https://github.com/expressjs/cors/blob/master/lib/index.js).
Now it is just a simple and opinionated cors middleware for Deno
[oak](https://deno.land/x/oak).

## Example

```typescript
import { CORS } from "https://deno.land/x/oak_cors@v0.1.0/mod.ts";
import { Application } from "https://deno.land/x/oak/mod.ts";

const app = new Application();
app.use(CORS());

// other middleware

await app.listen(":80");
```

If you use the default options, it will work as both `origin: true` and
`credentials: true`.
