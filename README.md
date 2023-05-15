# Eslint Config Nopersonalspace

After using this config, or versions of it, in nearly every project I work on I decided I should bundle it up into a shared package. This is a highly opinionated config, meant to be used more as an end product than a starting point.

## Usage

To use it, make sure to install it first with: `yarn add eslint-config-nopersonalspace -d`.

Then add it to your `.eslintrc.js` like follows.

```javascript
module.exports = {
  parser: "@typescript-eslint/parser",
  extends: ["eslint-config-nopersonalspace"],
};
```

## Notes

This config bundles all of it's eslint dependencies with it, which means you don't have to install any of the configs/plugins that it uses. However, this also means conflicts can happen if you try to extend this config too much. If you need to do that, I'd recommend just copy-pasting the eslint config from this repo into your own and doing it that way.
