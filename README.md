# Deprecated

**WARNING:** This project has moved to [@react-nano/redux-dynamic-modules](https://github.com/lusito/react-nano)

## redux-dynamic-modules-react-nano

[![Minified + gzipped size](https://badgen.net/bundlephobia/minzip/redux-dynamic-modules-react-nano)](https://www.npmjs.com/package/redux-dynamic-modules-react-nano)
[![NPM version](https://badgen.net/npm/v/redux-dynamic-modules-react-nano)](https://www.npmjs.com/package/redux-dynamic-modules-react-nano)
[![License](https://badgen.net/github/license/lusito/redux-dynamic-modules-react-nano)](https://github.com/lusito/redux-dynamic-modules-react-nano/blob/master/LICENSE)
[![Stars](https://badgen.net/github/stars/lusito/redux-dynamic-modules-react-nano)](https://github.com/lusito/redux-dynamic-modules-react-nano)
[![Watchers](https://badgen.net/github/watchers/lusito/redux-dynamic-modules-react-nano)](https://github.com/lusito/redux-dynamic-modules-react-nano)

Making [redux-dynamic-modules](https://github.com/microsoft/redux-dynamic-modules) more lightweight by using `react-redux-nano` instead of `react-redux`.
Written in TypeScript.

#### Why use redux-dynamic-modules-react-nano

- Very lightweight (see the badges above for the latest size).
- All it does is supply a different `DynamicModuleLoader` component which leverages the power of hooks in combination with `react-redux-nano`.
- You can use `redux-dynamic-modules-core` for the rest instead of `redux-dynamic-modules`.
- Only has four peer dependencies:
  - React 16.8.0 or higher
  - Redux 4.0.0 or higher
  - react-redux-nano 1.0.0 or higher
  - redux-dynamic-modules-core 5.0.0 or higher
- Liberal license: [zlib/libpng](https://github.com/Lusito/redux-dynamic-modules-react-nano/blob/master/LICENSE)

Note: Since this library uses `react-redux-nano`, your code also needs to be using `react-redux-nano` (otherwise you'd be using `redux-dynamic-modules`).

### Installation via NPM

```npm i redux-dynamic-modules-react-nano```

This library is shipped as es2015 modules. To use them in browsers, you'll have to transpile them using webpack or similar, which you probably already do.

### Examples

#### Loading Modules Dynamically

```tsx
import { DynamicModuleLoader } from "redux-dynamic-modules-react-nano";
export const MyComponent = () => (
    <DynamicModuleLoader modules={[myModule()]}>
        ....
    </DynamicModuleLoader>
);
```

### Report issues

Something not working quite as expected? Do you need a feature that has not been implemented yet? Check the [issue tracker](https://github.com/Lusito/redux-dynamic-modules-react-nano/issues) and add a new one if your problem is not already listed. Please try to provide a detailed description of your problem, including the steps to reproduce it.

### Contribute

Awesome! If you would like to contribute with a new feature or submit a bugfix, fork this repo and send a pull request. Please, make sure all the unit tests are passing before submitting and add new ones in case you introduced new features.

### License

redux-dynamic-modules-react-nano has been released under the [zlib/libpng](https://github.com/Lusito/redux-dynamic-modules-react-nano/blob/master/LICENSE) license, meaning you
can use it free of charge, without strings attached in commercial and non-commercial projects. Credits are appreciated but not mandatory.
