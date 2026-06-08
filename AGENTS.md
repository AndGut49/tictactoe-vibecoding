# AI Agent Instructions

## Project overview
This repository is a very small static Tic-Tac-Toe web app contained in a single `index.html` file.

- Uses React 17 / ReactDOM 17 via CDN imports.
- Implements the entire app with inline JavaScript and CSS in `index.html`.
- There is no `package.json`, build system, or test harness in the repository.

## What to do when editing
- Prefer minimal, incremental changes that keep the app self-contained unless the user explicitly asks to restructure the project.
- If adding features, maintain the existing single-page static setup and CDN-based React usage unless the user requests migration to a modern build tool.
- Keep Spanish UI labels and text consistent with the current app language.

## When to ask the user
- Before introducing a new project structure (e.g. splitting into separate JS/CSS files or adding npm tooling).
- Before adding automated tests or a build system when none already exist.

## Important details
- `index.html` is the only source file.
- The app renders into a root element with `ReactDOM.render(<App />, document.getElementById('root'))`.
- The game state lives in React state hooks and the winner logic is handled by `calculateWinner`.
