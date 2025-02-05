# Expo CLI Android Build Failure: Manifest Merger Errors

This repository demonstrates a common issue encountered when building Android APKs using the Expo CLI: manifest merger errors.  The problem typically arises from conflicts between AndroidX libraries or dependency version mismatches.

## Bug Description:

The Expo build process fails with the error "Execution failed for task ':app:processDebugManifest'. > Manifest merger failed with multiple errors, see logs."  Detailed error messages are usually provided in the build logs, often highlighting conflicts between library versions.

## Steps to Reproduce:

1.  Clone this repository.
2.  Run `expo prebuild`.
3.  Run `expo build:android`.

## Solution:

The solution usually involves resolving the conflicting library versions.  This often requires careful examination of the project's `package.json` file and potentially modifying the dependencies to ensure compatibility.  Check for duplicate AndroidX libraries and try upgrading to the latest versions.