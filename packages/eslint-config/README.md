# @thedaviddias/eslint-config

ESLint rules for all of my personal project.

## Installation

This module is distributed via [npm][npm] which is bundled with [node][node] and
should be installed as one of your project's `devDependencies`:

```bash
  npm install --save-dev @thedaviddias/eslint-config
```

This library has a required `peerDependencies` listing for [`eslint`][eslint]

## Usage

Then add the extends to your `.eslintrc.js`:

```javascript
module.exports = {
  extends: '@thedaviddias/eslint-config',
  rules: {
    // your overrides
  },
}
```

### Other configs

This config also exposes a few other configs that I use often and pull in as
needed.

You can use them standalone:

```javascript
module.exports = {
  extends: '@thedaviddias/<config-name>',
}
```

Or in combination with the base config (recommended)

```javascript
module.exports = {
  extends: ['@thedaviddias', '@thedaviddias/<config-name>'],
}
```

**Note**: Due to [this bug](https://github.com/eslint/eslint/issues/3458) you
need to have the associated plugins installed to make things work. I recommend
adding them as dependencies to your project if you're going to use the config
for it.

- `jest`: [jest](http://facebook.github.io/jest/) testing framework
- `jsx-a11y`:
  [eslint-plugin-jsx-a11y](https://github.com/evcohen/eslint-plugin-jsx-a11y)
  for rules regarding accessibility with JSX (_eslint-plugin-jsx-a11y_)
- `react`: [React](https://www.npmjs.com/package/react) JS library
  (_eslint-plugin-react_)
- `@typescript-eslint`:
  [@typescript-eslint/parser](https://www.npmjs.com/package/@typescript-eslint/parser)
  and
  [@typescript-eslint/eslint-plugin](https://www.npmjs.com/package/@typescript-eslint/eslint-plugin).

## Inspiration

This repo is heavily inspired inspired by
[eslint-config-kentcdodds](https://github.com/kentcdodds/eslint-config-kentcdodds)

<!-- prettier-ignore-start -->
[npm]: https://www.npmjs.com
[node]: https://nodejs.org
[prs-badge]: https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square
[prs]: http://makeapullrequest.com

[eslint]: https://github.com/eslint/eslint
<!-- prettier-ignore-end -->
