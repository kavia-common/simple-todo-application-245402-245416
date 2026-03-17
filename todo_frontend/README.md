# Todo Frontend (React)

This folder contains the React frontend application (Create React App). In the current repository state, the UI is a lightweight template that demonstrates a light/dark theme toggle and basic styling.

## Features (current)

The current implementation includes:

- A light/dark theme toggle that sets the `data-theme` attribute on the document root.
- A minimal responsive layout and theme variables implemented in `src/App.css`.
- Standard Create React App scripts for running, testing, and building.

## Local development

1. Install dependencies:

   ```bash
   npm install
   ```

2. Run the app:

   ```bash
   npm start
   ```

Then open `http://localhost:3000`.

## Configuration (environment variables)

This frontend supports configuration via environment variables. The container defines the following variables (they are optional unless your deployment requires them):

- `REACT_APP_API_BASE`: Base path/URL for API requests (if/when the frontend is wired to a backend).
- `REACT_APP_BACKEND_URL`: Backend base URL (if used).
- `REACT_APP_FRONTEND_URL`: Public frontend URL (if used in redirects or links).
- `REACT_APP_WS_URL`: WebSocket URL (if used).
- `REACT_APP_NODE_ENV`: Environment mode (commonly `development` or `production`).
- `REACT_APP_NEXT_TELEMETRY_DISABLED`: Reserved; may be used in some hosting setups.
- `REACT_APP_ENABLE_SOURCE_MAPS`: Control source map generation (commonly `true`/`false` depending on your build tooling).
- `REACT_APP_PORT`: Port to run the dev server on (note that Create React App typically uses `PORT`; if you use `REACT_APP_PORT`, ensure your start command maps it appropriately).
- `REACT_APP_TRUST_PROXY`: Reserved; may be used in some hosting setups.
- `REACT_APP_LOG_LEVEL`: Reserved; may be used to control client-side logging.
- `REACT_APP_HEALTHCHECK_PATH`: Reserved; may be used by hosting/health-check tooling.
- `REACT_APP_FEATURE_FLAGS`: Reserved; may be used to enable/disable UI features.
- `REACT_APP_EXPERIMENTS_ENABLED`: Reserved; may be used to enable experimental features.

To set variables locally, create a file named `.env` in this folder (`todo_frontend/.env`) and restart the dev server after changes.

## Available scripts

- `npm start`: Runs the app in development mode.
- `npm test`: Launches the test runner.
- `npm run build`: Builds the app for production.
- `npm run eject`: Ejects Create React App configuration (irreversible).

## UI theming notes

The theme is controlled by a `data-theme` attribute on the root `<html>` element.

- Theme logic: `src/App.js`
- Theme variables and styles: `src/App.css`

## Learn more

- React documentation: https://reactjs.org/
- Create React App documentation: https://create-react-app.dev/
