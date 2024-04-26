# YARN MODERN

mordern yarn, after v2, workspace system is changed.
Modern yarn recognize workspace packages without workspaces option. However, workspace function such as `focus` does'not work.

## Conditions

-  "workspaces" in package.json must be set array.

>![INFO]
> `private` must not be true.

## Installation Scripts

### at root

"-W" option is useless after v2.

```
yarn add example
```

### child packages

same above.

### Add workspace package

add "workspace-package" to "workspaces" array manually.
"workspace-package" is recognized by package.json workspace option.

