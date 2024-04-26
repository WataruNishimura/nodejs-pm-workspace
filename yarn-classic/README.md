# YARN CLASSIC WORKSPACE PROJECT

## Conditions

- "private" in package.json must be true.
- "workspaces" in package.json must be set array or empty array.
  - workspaces array does not need to includes some package string.
  - workspaces array does not accept nullish value except empty array such as "null", '""'.

## Installation scripts

### at root

"-W" options is needed at project root. W is CAPITAL.

```
//e.g.
yarn add -W example
```

### child packages

Just exectute `yarn add`.

## Add workspace pacakge

add "workspace-package" to "workspaces" array manually.
"workspace-package" is recognized by package.json workspace option.
