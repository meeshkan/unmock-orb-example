# Unmock orb example

[![CircleCI](https://circleci.com/gh/unmock/unmock-orb-example.svg?style=svg)](https://circleci.com/gh/unmock/unmock-orb-example)

Example repository using [unmock](https://unmock.io) for tests and [Unmock orb](https://circleci.com/orbs/registry/orb/unmock/unmock) for test reports.

This is a Node.js application running an [Express](https://expressjs.com/) server and using [React](https://reactjs.org/) for server-side rendering. The application displays a list of **your** GitHub repositories (that's you, the developer).

## Instructions

### Running the application locally

1. Create a new personal GitHub [access token](https://github.com/settings/tokens) with read access to your repositories
1. Set the environment variable `GITHUB_TOKEN` in `.env` file (see `.env.example` for an example)
1. Install dependencies: `yarn` (or `npm i`)
1. Run the development server with hot reloading: `yarn dev`
1. Navigate to [localhost:3000](http://localhost:3000)
1. To build the app and run in production mode: `yarn build && yarn start`

### Running tests

Run tests:

```bash
$ yarn test
```

Running tests **does not require creating a GitHub access token**: they use Unmock to mock calls to the GitHub API!
