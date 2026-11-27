# Chess-Coach

A Next.js app that coaches you on your chess.com games.

## Requirements

- [Node.js](https://nodejs.org/) 24 (pinned in [`.nvmrc`](.nvmrc))
- npm (comes with Node.js)

If you use [nvm](https://github.com/nvm-sh/nvm), run `nvm use` in the project root to switch to the right version.

## Install

```bash
git clone <repo-url>
cd chess-coach
npm install
```

## Environment variables

Copy the example file and fill in the values:

```bash
cp .env.example .env
```

| Variable            | Description                                         |
| ------------------- | --------------------------------------------------- |
| `CHESSCOM_API_KEY`  | API key used to access chess.com data.              |
| `CHESSCOM_USERNAME` | The chess.com username whose games are analysed.    |
| `LLM_PROVIDER`      | Which LLM provider generates the coaching feedback. |
| `LLM_API_KEY`       | API key for the chosen LLM provider.                |
| `DATABASE_URL`      | Connection string for the database.                 |

`.env` files are git-ignored. Never commit real keys; only `.env.example` is tracked.

## Run

```bash
npm run dev     # start the dev server at http://localhost:3000
```

For a production build:

```bash
npm run build   # build the app
npm run start   # serve the production build
```

## Test and check

```bash
npm run lint           # ESLint
npm run typecheck      # TypeScript strict type check (tsc --noEmit)
npm run format:check   # check formatting with Prettier
npm run format         # fix formatting with Prettier
```

Run all checks before opening a pull request. Unit tests will live in [`tests/`](tests/); a test runner has not been added yet.

## Project structure

```text
src/
  app/          Next.js App Router pages and layouts
  components/   Reusable React components
  lib/          Shared logic and helpers
tests/          Tests
public/         Static assets
```

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md).

## License

[MIT](LICENSE)
