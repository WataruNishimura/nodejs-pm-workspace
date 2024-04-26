# Node.js package manager workspace recognition.

This repository is for examining how node.js package manager function recognizes as it is.

Please use this repositroy for developing like cli tool with node.js package managers' workspace function.

## Contribution

If anything wrong is found, please create pr.
I welcome such contritbutions.

## Installation scripts

### at root

Just execute `yarn add`.

### child package

Just execute `yarn add` from package directory, or use `yarn workspaces focus`.

>![WARN]
> if you need to install dependencies with `--production` option, you must use `yarn workspaces focus -A --production` after v2. 
> This commands means "install only save dependencies to all packages."


# Owner

[Wataru Nishimura](https://x.com/_n13u_)