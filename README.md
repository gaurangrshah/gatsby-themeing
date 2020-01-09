# WIP

## 👷‍♂️🚧🏗

Currently have working mdx editor theme as per: [egghead](https://egghead.io/lessons/vue-js-introduction-to-mdx?pl=building-websites-with-mdx-and-gatsby-161e9529)

forked that to a seperate theme, to run:
~/package.json:


```json
{
  "private": true,
  "workspaces": [
    "gatsby-theme-mdx-editor",
    "site"
  ]
}

```

~/site/package.json:
```json
  "dependencies": {
    "gatsby-theme-mdx-editor": "*",
  }
```

~/site/gatsby-config.js

```js
module.exports = {
  plugins: [`gatsby-theme-mdx-editor`]
}
```

Run yarn to ensure the packages' relationships are set properly.
```shell
yarn
```

```shell
  yarn workspace site develop
```

Alternatively you could update the theme using:
```shell
  yarn workspace gatsby-theme-mdx-editor develop
```
