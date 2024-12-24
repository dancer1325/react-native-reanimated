## Running the MacOSExample app

* | project's root directory
  ```
  yarn install
  ```
* | this directory
  ```
  yarn install
  ```
* | `ios` -- TODO: NOT exist ❌

  ```
  pod install
  ```
* | `macos`

  ```
  pod install
  ```
* | this directory

  ```
  yarn start
  
  # input "i", "a", "d" or "r" 
  ```

### Running | macOS

* ways
  * open the workspace | Xcode

    ```
    open macos/MacOSExample.xcworkspace
    ```

  * build and run directly -- from the -- CL

    ```
    yarn react-native run-macos
    ```

### Troubleshooting

* if you have problems building the app -> | `macos/`

  ```
  rm -rf Pods Podfile.lock build
  ```
