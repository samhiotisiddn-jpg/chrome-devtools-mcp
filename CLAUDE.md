# Chrome DevTools MCP

MCP server and CLI for Chrome DevTools Protocol (CDP). Enables AI agents to control browser instances, inspect pages, run JavaScript, and capture screenshots via the Model Context Protocol.

## Quick Reference

```bash
npm run build       # compile TypeScript
npm run test        # build + run all tests
npm run test tests/McpContext.test.ts  # single test file
npm run format      # fix formatting + lint errors
```

## Project Structure

- `src/` — TypeScript source
  - `server.json` — MCP server manifest
  - `gemini-extension.json` — Gemini extension config
- `tests/` — test suite (`.test.ts` files)
- `scripts/` — auxiliary scripts
- `docs/` — documentation
- `rollup.config.mjs` — bundler config
- `tsconfig.json` — TypeScript config
- `eslint.config.mjs` — linting rules

## TypeScript Rules

- No `any` type — ever.
- No `as` type casts.
- No `!` non-null assertions.
- No `@ts-ignore`, `@ts-nocheck`, or `@ts-expect-error` comments.
- Prefer `for...of` over `forEach`.

## Testing

Run all tests before marking work complete: `npm run test`. Run a single file with `npm run test path/to/file.test.ts`.

## Commit & PR Guidelines

- Conventional commit style: `feat:`, `fix:`, `chore:`, etc.
- Keep commits focused; one logical change per commit.
- Format code (`npm run format`) before committing.
