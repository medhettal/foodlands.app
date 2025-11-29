# foodlands.app

Short on-ramp checklist to get the project running locally.

## Prerequisites
- Git installed
- One of the language runtimes below depending on which part of the repo you use:
  - Node.js (LTS) and npm / yarn
  - Python 3.8+ and virtualenv / venv
  - Flutter SDK (stable) for mobile clients

## Quick setup (general)
1. Clone repository
   - git clone git@github.com:medhettal/foodlands.app.git
   - cd foodlands.app
2. Create a local env file from the example:
   - cp .env.example .env
   - Fill in values in `.env` (do NOT commit secrets)

## Node (if the project contains Node code)
- Install dependencies:
  - npm install
  or
  - yarn install
- Run locally:
  - npm start
- Build:
  - npm run build
- Tests:
  - npm test
- Lint:
  - npm run lint

## Python (if applicable)
- Create venv and install:
  - python -m venv .venv
  - source .venv/bin/activate  # macOS / Linux
  - .venv\Scripts\activate     # Windows (PowerShell)
  - pip install -r requirements.txt
- Run:
  - python -m your_module
- Tests:
  - pytest

## Flutter (if applicable)
- Install Flutter SDK: https://flutter.dev/docs/get-started/install
- Get packages:
  - flutter pub get
- Run (simulator / device):
  - flutter run
- Build:
  - flutter build apk
- Tests:
  - flutter test

## Environment variables
- Use `.env.example` as a template. DO NOT commit real secrets to the repository. Use CI secrets or a secrets manager for production keys.

## Next steps (suggested)
- Identify the primary language / runtime used in this repo and add a focused "Getting started" section.
- Add a more specific CI workflow (install, build, test) once the main stack is known.
- Add contributor / code-style guidelines, and a troubleshooting section.

## Contacts
- Repo owner: @medhettal
