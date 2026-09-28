# tinqerjs.org

Tinqer documentation site, generated from the sibling `tinqer` repository.

## Development

Use Node.js 22.13+ in the 22.x line, or Node.js 24+, and npm 11.19+.
Verification uses Node.js 26. Keep the two repositories as siblings so the
builder can read the library's current documentation.

```sh
npm ci
npm run build
npm run serve
```

- [Local documentation preview](http://localhost:4567)

The project `.npmrc` enforces a seven-day minimum release age and strict engine
checks so older npm versions cannot silently ignore the policy. Do not bypass
these safeguards when updating dependencies. Commit regenerated `build/` artifacts together
with their dependency and source changes; a local build does not deploy them.
