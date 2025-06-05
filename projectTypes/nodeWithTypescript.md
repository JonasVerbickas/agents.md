Make sure all dependencies are present by:

```bash
npm ci
```

Whenever implementing new logic use TDD -- introduce vitest unit tests in corresponding `.spec.ts` files.
To run unit tests:

```bash
npm run test
```

Before commiting anything make sure your code passes expected code style:

```bash
npm run format
npm run lint
npm run typecheck
```
