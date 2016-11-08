# Express & mongoose REST API Boilerplate in ES6 with Code Coverage

## Overview

This is a boilerplate application for building REST APIs in Node.js using ES6 and Express with Code Coverage and JWT Authentication. Helps you stay productive by following best practices. Follows [Airbnb's Javascript style guide](https://github.com/airbnb/javascript).

## Getting Started
Clone the repo:
```sh
git clone git@github.com:ram-dev/es6restapi.git
cd es6restapi
```

Install dependencies:
```sh
npm install
```

Start server:
```sh
# Start server
npm start


Tests:
```sh
# Run tests written in ES6 along with code coverage
npm test

# Run tests on file change
npm run test:watch

# Run tests enforcing code coverage (configured via .istanbul.yml)
npm run test:check-coverage
```

Lint:
```sh
# Lint code with ESLint
npm run lint

# Run lint on any file change
npm run lint:watch
```

Other gulp tasks:
```sh
# Wipe out dist and coverage directory
gulp clean

# Default task: Wipes out dist and coverage directory. Compiles using babel.
gulp
```

##### Deployment

```sh
# compile to ES5
1. npm run build

# upload dist/ to your server
2. scp -rp dist/ user@dest:/path

# install production dependencies only
3. npm i --production

# Use any process manager to start your services
4. pm2 start dist/index.js

In production you need to make sure your server is always up so you should ideally use any of the process manager recommended [here](http://expressjs.com/en/advanced/pm.html).
We recommend [pm2](http://pm2.keymetrics.io/) as it has several useful features like it can be configured to auto-start your services if system is rebooted.