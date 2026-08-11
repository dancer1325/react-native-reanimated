---
sidebar_position: 1
---

## Prerequisites

* [React Native New Architecture (Fabric)](https://reactnative.dev/architecture/landing-page)
  * Reason:🧠NOT tested | Legacy Architecture (Paper)🧠 

## Installation

### Step 1: Install the package

```bash
npm install react-native-worklets
---
yarn add react-native-worklets
---
pnpm add react-native-worklets
---
bun add react-native-worklets
```

### Step 2: | your Expo project, rebuild native dependencies

* prebuild
  * == update the native code | 
    * "ios/"
    * "android/"

    ```bash
    npx expo prebuild
    ---
    yarn expo prebuild
    ---
    pnpm expo prebuild
    ---
    bunx expo prebuild
    ```

### | use [React Native Community CLI](https://github.com/react-native-community/cli)

* | your "babel.config.js",
  * add the `react-native-worklets/plugin` plugin 

    ```js {7}
    module.exports = {
      presets: [
        ... // don't add it here :)
      ],
      plugins: [
        ...
        'react-native-worklets/plugin',
      ],
    };
    ```
    * [options](../worklets-babel-plugin/options.md)

TODO:

<details>
  <summary>Why do I need this?</summary>

  In short, the Worklets babel plugin automatically converts special JavaScript functions
  (called [worklets](/docs/fundamentals/glossary#worklet)) to allow them to be passed and run on the [Worklet Runtimes](/docs/fundamentals/runtimeKinds#worklet-runtime)

  Since [Expo SDK 54](https://expo.dev/changelog/sdk-54-beta#notable-breaking-changes), the Expo starter template includes the Worklets babel plugin by default.

  To learn more about the plugin head onto to [Worklets babel plugin](/docs/worklets-babel-plugin/about) section.
</details>

#### Clear Metro bundler cache (recommended)

```bash
npm start -- --reset-cache
---
yarn start --reset-cache
---
pnpm start --reset-cache
---
bun start --reset-cache
```

#### Android

No additional steps are necessary.

#### iOS

While developing for iOS, make sure to install [pods](https://cocoapods.org/) first before running the app:

```bash
cd ios && pod install && cd ..
```
