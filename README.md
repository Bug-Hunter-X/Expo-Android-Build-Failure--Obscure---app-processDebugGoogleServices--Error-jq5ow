# Expo Android Build Failure: Obscure ':app:processDebugGoogleServices' Error

This repository demonstrates a bug encountered during the Android build process using Expo CLI. The build fails with the error message `Execution failed for task ':app:processDebugGoogleServices'`, lacking specific details to aid in debugging.  This issue occurs even when following standard Expo documentation.

## Bug Reproduction

1. Clone this repository.
2. Navigate to the project directory in your terminal.
3. Run `expo prebuild`. 
4. Attempt to build an Android APK using `expo build:android`.
5. Observe the build failure with the vague error message.

## Solution

The solution involves verifying the `google-services.json` file's validity and correctness, verifying dependencies and making sure they match what's defined in the project's `package.json`, and cleaning the project's build files.
