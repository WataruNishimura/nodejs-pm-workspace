# NPM

the most common way to use package manager in node.js.

## Conditions

- "workspaces" in package.json must be set array.
  - workspaces array does not need to includes some package string.
  - if workspaces is not array, npm throw errors

## Installation scripts

### at root

Just execute `npm install`

### child package

Just execute `npm install`, or use `npm install --workspace={workspace_folder}`.

## Add workspace package

`npm init -w {child_package_directory}` commands create, add or link sub package with this command.