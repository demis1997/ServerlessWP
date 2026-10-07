# ServerlessWP starter fork

Fork of [mitchmac/ServerlessWP](https://github.com/mitchmac/ServerlessWP): an experimental WordPress starter whose JavaScript handler routes requests through the `serverlesswp` PHP runtime. Source and the existing [license](LICENSE) retain their upstream attribution. This fork is not claimed as an independently developed hosting platform.

## Inspected configuration

`api/index.js` stages the WordPress directory under `/tmp/wp` and calls the runtime. `util/install.js` checks database configuration. Copy [`.env.example`](.env.example) only into an ignored local environment file; real database credentials must stay private.

The manifest declares Node `18.x` and `serverlesswp ^0.1.2`, with no test/build scripts or committed npm lockfile. Installation can be explored in an isolated checkout:

```sh
npm install --ignore-scripts
```

This command was inspected, not executed. Modern runtime compatibility, PHP/native dependencies, database connectivity and hosting behavior remain unverified. No deployment was performed. The repository has no independently verified local application-start command.

## Historical documentation

Useful original setup and attribution are retained in [historical upstream notes](docs/HISTORICAL_SETUP.md). Their free-tier, pricing and platform claims are not current verified recommendations. Review official provider documentation before choosing hosting or deploying this experimental starter.
