# Gelato Assignment

## Overview
This project is used to test [ToDo Application](https://todomvc.com/examples/react/#/). The automation uses Cypress Tool. 
Test cases are written in JavaScript with Cucumber BDD framework and Chai assertions. 
Test cases are specified in `cypress\integration\features` folder.
Tool uses multiple-cucumber-html-reporter tool for generating report.


## Installation

```bash
## install all dependencies from the root directory
npm install
```

## Opening Cypress GUI

```bash
# Open Cypress GUI
npm run cypress:open
```

## Running from the CLI

Install dependencies with `npm install` or `npm ci`

See scripts in `package.json` to run the tests.

* `cypress:info` - Displays Cypress information.
* `test:run` - Runs Cypress test in headless mode.
* `test:run-headed` - Runs Cypress test in head mode.
* `test:chrome` - Runs Cypress test in chrome browser in head mode.

## Report Generation
Run below command from `root folder` to generate Cucumber-HTML report.

```bash
node cypress/cucumber-html-report.js
```

Reports are generate at below location
```
.\cypress\report\index.html
```