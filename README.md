<img src="public/icon.png" width="128px" alt="Icon" />

# Webpack Boilerplate

A good starting point for using [webpack](https://webpack.js.org/) to build stuffs.

## Compatibility

Tested on both _Windows_ and _macOS_, with:

- `Node` = `16.15.1`
- `Yarn` = `3.2.4`

## Features

- Fully customizable webpack-based building system.
- Support webpack 5, React 18, TypeScript, Sass, Less, Tailwind CSS, etc.
- Support [Hot Module Replacement (HMR)](https://webpack.js.org/concepts/hot-module-replacement/).
- Support [ESLint](https://www.npmjs.com/package/eslint), [stylelint](https://www.npmjs.com/package/stylelint), and [Prettier](https://www.npmjs.com/package/prettier).
- Support [husky](https://www.npmjs.com/package/husky), [lint-staged](https://www.npmjs.com/package/lint-staged), and [commitlint](https://www.npmjs.com/package/@commitlint/cli).

## How to Use

### 1. Update Configurations

- Edit `webpack.config.js` and update the configuration field `entry` to determine what to be built;

### 2. CLI Commands

```bash
# Install dependencies
yarn install

# Start dev server
yarn run start

# Build application
yarn run build

# Commit
yarn commit

# Release
yarn release
```

## Hot Module Replacement (HMR)

To use [Hot Module Replacement](https://webpack.js.org/concepts/hot-module-replacement/), please place components outside of the top-level file. Components in the top-level file will be downgraded to _live reload_.

## Class Names in CSS-Modules

CSS's naming convention requires the class names to be in `kebab-case`. However, in JavaScrip, it is not allowed to write `style.my-style` and only accepts `style['my-style']` or `style.myStyle`. It is not convenient. Therefore, in this boilerplate, the class names in css-modules will be converted from `kebab-case` to `camelCase` to allow usages such as `style.myStyle`. 

## Credits

- <div>Icons made by <a href="https://www.flaticon.com/authors/freepik" title="Freepik">Freepik</a> from <a href="https://www.flaticon.com/" title="Flaticon">www.flaticon.com</a></div>
