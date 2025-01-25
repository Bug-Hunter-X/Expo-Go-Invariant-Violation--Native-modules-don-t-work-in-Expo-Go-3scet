# Expo Go Invariant Violation: Native modules don't work in Expo Go
This repository demonstrates a bug where a custom native module works on a physical device but fails in Expo Go with the error: `Invariant Violation: Native modules don't work in Expo Go`.

## Bug Description
The app uses a custom native module to access device functionality not available through the Expo APIs. The app functions correctly when built and run on a physical device. However, when attempting to run the same app through Expo Go, it crashes with the aforementioned error message.  This is a known limitation of Expo Go.

## Solution
The solution is to avoid using custom native modules when developing for Expo Go.  For development and testing purposes, you should focus on using the Expo APIs, or explore EAS Build for testing your app's functionality with native modules.   Expo Go is primarily intended for testing JavaScript-only functionality.

## Setup
1. Clone the repository
2. `npm install` or `yarn install`
3. Attempt to run in Expo Go and observe the error. 
4. (To test solution) Update to use Expo APIs instead of Native Module.
