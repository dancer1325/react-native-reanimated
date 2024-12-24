## Running the Example app

1. | root, install node_modules

    ```
    yarn
    ```

2. Build the library

   ```
   yarn build
   ```

3. | `Example/`, install node_modules

   ```
   cd Example
   yarn
   ```

4. | `apps/*-example/ios/`, install Pods

   ```
   cd ios
   pod install
   ```

5. | `apps/*-example/`, start Metro bundler

   ```
   cd ..
   yarn start
   ```

### Running | iOS

You can either open the workspace in Xcode and launch the app from there:

```
open ios/ReanimatedExample.xcworkspace
```

or build and run directly from the command line:

```
yarn react-native run-ios
```

**Important:** You will need to have an iOS device or simulator connected.

### Running | Android

You can either open the project with Android Studio and launch the app from there:

```
open -a "Android Studio" android/
```

or build and run directly from the command line:

```
yarn react-native run-android
```

**Note:** You can also pass `--active-arch-only` flag to build the app only for the current architecture to significantly shorten build time.

**Important:** You will need to have an Android device or emulator connected.
