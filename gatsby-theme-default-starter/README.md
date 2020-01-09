# WIP

## 👷‍♂️🚧🏗

Currently have working theme based on the gatsby-default-starter

forked that to a seperate theme, to run:

~/package.json:

```json
{
  "private": true,
  "workspaces": [
    "gatsby-theme-default-starter",
    "site"
  ]
}

```

~/site/package.json:
```json
  "dependencies": {
    "gatsby-theme-default-starter": "*",
  }
```

~/site/gatsby-config.js

```js
module.exports = {
  plugins: [`gatsby-theme-default-starter`]
}
```

Run yarn to ensure the packages' relationships are set properly.
```shell
yarn
```

To consume the theme:
```shell
  yarn workspace site develop
```

Alternatively you could update the theme using:
```shell
  yarn workspace gatsby-theme-default-starter develop
```


Create pages in `site/src/pages` to override the default theme