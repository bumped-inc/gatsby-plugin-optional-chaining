# Optional chaining support for Gatsby's Babel config

## Description

It enables the optional chaining operator (`a ?. b`): [see the TC39 proposal](https://github.com/tc39/proposal-optional-chaining)

## How to install

Install the plugin and its dependencies :

```bash
npm i @bumped-inc/gatsby-plugin-optional-chaining @babel/core @babel/plugin-proposal-optional-chaining
```

or

```bash
yarn add @bumped-inc/gatsby-plugin-optional-chaining @babel/core @babel/plugin-proposal-optional-chaining
```

Add the plugin in `gatsby-config.js`:

```js
module.exports = {
  plugins: [
    // other plugins
    '@bumped-inc/gatsby-plugin-optional-chaining',
  ],
}
```

## Examples of usage

```js
const maybeObj = null;
const result = maybeObj?.value; // result: undefined

const actualObj = { value: 5 };
const betterResult = actualObj?.value // betterResult: 5
```
