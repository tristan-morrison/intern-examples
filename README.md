This repo provides a minimal repro setup for issue [#146002](https://github.com/microsoft/vscode/issues/146002) in the VS Code [repo](https://github.com/microsoft/vscode). The issue involves apparent freezing/hanging of the VS Code debugger when debugging an app in the browser using the integrated console.

The repro case provided here is taken from the repo https://github.com/theintern/intern-examples — specifically, from the package `typescript-example` within that repo. The original README for that package is reproduced below.

---------------------

# typescript-example

This example uses Intern to test a jQuery + Backbone TodoMVC app written in TypeScript.

## Setup

1. Install the JRE or JDK
   This demo runs with local Selenium, which Intern will automatically install.

2. Install node modules

    ```
    npm install
    ```

## Running tests

* **From a browser**

    ```
    npm start
    ```

    Navigate to `http://localhost:9000/__intern/`

* **Using WebDriver**

    ```
    npm test
    ```

The `npm test` command will run tests in Chrome by default. The test config in this project contains convenience configurations for other browsers as well.

```
npm test config=@edge
npm test config=@firefox
npm test config=@ie
npm test config=@safari
```
