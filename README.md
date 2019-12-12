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

### See the orb in action

Take a look at PR [#1](https://github.com/unmock/unmock-orb-example/pull/1). The orb publishes Unmock test report and sends a link to the report for inspection.

## Contributing

If you notice an error or you'd like to add something new to this example, please [open an issue](https://github.com/unmock/unmock-orb-example/issues). We really appreciate the feedback and support! 

Please note that this project is governed by the [Unmock Community Code of Conduct](https://github.com/unmock/code-of-conduct). By participating in this project, you agree to abide by its terms.
