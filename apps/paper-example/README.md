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

* ways
  * open the workspace | Xcode

     ```
     open ios/ReanimatedExample.xcworkspace
     ```

  * build and run directly -- from the -- CL

     ```
     yarn react-native run-ios
     ```
    * Problems: "error Failed to build ios project. "xcodebuild" exited with error code '70'. "
      * Solution: TODO:

### Running | Android

* ways
  * open the project -- via -- Android Studio & launch the app from there or

    ```
    open -a "Android Studio" android/
    ```

  * build and run directly -- from the -- CL

    ```
    yarn react-native run-android
    ```
    * Problems:
      * Problem1: NOTHING start up
        * Solution: TODO:
    * if you want to speed up ALL -> run

    ```
    yarn react-native run-android --active-arch-only
    ```
   