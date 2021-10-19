# Contributing

Suggestions, bug reports, and pull requests welcome.

## About This Extension

This extension uses the TextMate language definition from https://github.com/kotfu/Bunch.tmbundle/blob/main/Syntaxes/Bunch.tmLanguage. This language definition is copied and committed here when it is updated.


## Prerequisites

In order to publish this extension you need to:

- Install [Node.js](https://nodejs.org/en/)
- Use `npm` to install `vsce`
    ```
    $ npm install vsce
    ```


## Publishing a Release

To make it easier for users to find and install, this extension is published to
the [Visual Studio Code Marketplace](https://marketplace.visualstudio.com/VSCode). [Publishing Extensions](https://code.visualstudio.com/api/working-with-extensions/publishing-extension) explains the details of how it works and how to do it.

Here's the process:

1. Commit all your changes and push them to github
2. Decide on the new version for the release
3. Update CHANGELOG.md with the new version and commit it
4. Publish to the VSCode Marketplace with:
     ```
     $ npx vsce publish {version}
     ```
   This will update `package.json` with the new version number and create a
   git tag for the release
5. Push the repo to github
