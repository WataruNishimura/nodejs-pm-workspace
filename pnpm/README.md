# PNPM

pnpm workspace is deference from other managers.
pnpm recognize workspaces by `pnpm-workspace.yaml`.
`workspace` in package.json and other files are ignored.

## Conditions

- "pnpm-workspace.yaml" exists.
  - pnpm recognize as workspace even it is empty. So, if you try to add dependency at project root, you will fail.
- All sub directory are recognized as sub package by default.
- write sub packages by yaml, in detail, read [official docs](https://pnpm.io/ja/pnpm-workspace_yaml).
  ```
  packages:
  # all packages in direct subdirs of packages/
  - 'packages/*'
  # all packages in subdirs of components/
  - 'components/**'
  # exclude packages that are inside test directories
  - '!**/test/**'
  ```

## Installation Scripts

### at root

you need to apply "-w" option.

```
pnpm add {dependency_name} -w
```

### child packgages

Just execute `pnpm add`.

### Add workspace 

add "workspace-package" to "packages" yaml array manually.