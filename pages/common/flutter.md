# flutter

> Google's cross-platform SDK for building apps from a single codebase.
> Some subcommands such as `pub` have their own usage documentation.
> More information: <https://docs.flutter.dev/reference/flutter-cli>.

- Verify the toolchain and list any setup issues:

`flutter doctor {{[-v]}}`

- List all connected devices, emulators, and simulators:

`flutter devices`

- Run the app on a specific device (builds and installs it):

`flutter run {{[-d]}} {{device_id}}`

- Attach the debugger to an already-running app (hot reload/inspect):

`flutter attach {{[-d]}} {{device_id}}`

- Run in profile or release mode instead of debug:

`flutter run --{{profile|release}} {{[-d]}} {{device_id}}`

- Install a prebuilt app onto a device without launching it:

`flutter install {{[-d]}} {{device_id}}`

- Build for Android (installable APK or Play Store bundle):

`flutter build {{apk|appbundle}} --release`

- Build for iOS, web, or desktop:

`flutter build {{ios|ipa|web|macos|windows|linux}} --release`
