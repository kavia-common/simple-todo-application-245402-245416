# Simple Todo Application

This repository contains a React frontend application.

## Project structure

The main application lives in:

- `todo_frontend/`: React (Create React App) frontend

## Getting started (frontend)

1. Change into the frontend directory:

   ```bash
   cd todo_frontend
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

3. Start the development server:

   ```bash
   npm start
   ```

The app will be available at `http://localhost:3000` by default.

## Environment variables

The frontend supports configuration via environment variables (Create React App-style `REACT_APP_*` variables). The following variables are defined for this container:

- `REACT_APP_API_BASE`
- `REACT_APP_BACKEND_URL`
- `REACT_APP_FRONTEND_URL`
- `REACT_APP_WS_URL`
- `REACT_APP_NODE_ENV`
- `REACT_APP_NEXT_TELEMETRY_DISABLED`
- `REACT_APP_ENABLE_SOURCE_MAPS`
- `REACT_APP_PORT`
- `REACT_APP_TRUST_PROXY`
- `REACT_APP_LOG_LEVEL`
- `REACT_APP_HEALTHCHECK_PATH`
- `REACT_APP_FEATURE_FLAGS`
- `REACT_APP_EXPERIMENTS_ENABLED`

If you are running locally, you can place these in `todo_frontend/.env` (not committed) or provide them through your environment when starting the app.

## Available scripts (frontend)

From inside `todo_frontend/`:

- `npm start`: Run the app in development mode.
- `npm test`: Run tests.
- `npm run build`: Build for production.
- `npm run eject`: Eject Create React App configuration (irreversible).

## Notes

The current frontend code in this repository is a basic React app template with a light/dark theme toggle. If additional todo features are added (add, complete, delete, filtering, localStorage persistence), this README should be updated to reflect the implemented behavior.
