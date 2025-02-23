# React Native Dimensions API Inaccuracy on Android

This repository demonstrates a common issue encountered when using the `Dimensions` API in React Native to retrieve screen dimensions, specifically on Android devices with different screen densities.  The problem manifests as inaccurate width and height values, leading to layout problems.

## Problem

The `Dimensions.get('window')` method may return incorrect dimensions, especially when the app is run on a device with a screen density different from the one used during development. This can cause elements to be rendered incorrectly, clipped, or positioned inappropriately.

## Solution

The solution involves using `PixelRatio` to adjust the dimensions based on the device's screen density. This ensures consistent layout across different devices.

## Usage

1. Clone the repository.
2. Run `npm install` or `yarn install`.
3. Run the app on various Android devices to observe the difference.