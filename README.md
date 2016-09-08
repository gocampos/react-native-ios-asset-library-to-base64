# react-native-ios-asset-library-to-base64
# https://github.com/dinesh829269/react-native-ios-asset-library-to-base64.git
A React Native Module that converts an image's asset-library:// uri to base64:

## Install

### IOS
1. `npm install --save react-native-ios-asset-library-to-base64`
2. In the XCode's "Project navigator", right click on your project's Libraries folder ➜ `Add Files to <...>`
3. Go to `node_modules` ➜ `react-native-asset-library-to-base64` ➜ `ios` ➜ select `AssetLibraryToBase64.m`
4. Make sure `AssetLibraryToBase64.m` is listed under 'Compile Sources' in your project's 'Build Phases' tab
5. Compile

## Usage

1. In your React Native javascript code, bring in the native module:

var ReadImageData = require('NativeModules').ReadImageData;

2. convert image url:

// image asset-library:// uri
ReadImageData.readImage(uri, (imageBase64) => {
  console.log(imageBase64);
});
  ```

## Source
This code was copied from https://github.com/scottdixon/react-native-upload-from-camera-roll/blob/master/RCTCustom.m and https://medium.com/@scottdixon/react-native-creating-a-custom-module-to-upload-camera-roll-images-7a3c26bac309#.xckz6wr87.  I just took the example and turned it into a module for ease of use.
