# zapp-reactnative-starter

## to Run project locally, do not forget to start metrro bundler server
```
yarn start
- optional (--clear-cache)
```
# Zapp React Native Starter Project
## Motivation
The motivation of the project is to serve as a simple to run, simple to edit clean React Native project for Zapp Plugins.

This repository is a template for anybody to clone and start building a RN Plugin for Zapp.

## Current Contents
This template repository contains the following:
* React native app based on RN 0.59 with 1 screen containing a headline and a printout of the initial props
* Sample plugin manifest
* This guide

## Running the ReactNative bundle
In order to run this project simply:
* run either `npm i` or `yarn`
* run `react-native start`

## Building deployable files
This repository contains basic build scripts that will output to the following structure:
```
 <project_folder>/build/android
 <project_folder>/build/ios
```
In order to build run either `npm run-script build` or `yarn build`.

## Testing within an Applicaster App - iOS
For the sake of simplicity and quick testing - Zapp already contains an app with this plugin built in.
With the following steps you could run your local version of the plugin within a full fledged Zapp App enviornment.

1. If you have access to Zapp - please use the following app family: https://zapp.applicaster.com/app_families/1554
2. If you don't have access to zapp - Feel free to download the compiled version: https://rink.hockeyapp.net/apps/e96cb5f66bb34ad99e0d10bdf2637ce0
3. Install the app on the device and run it
4. Go to device settings app -> Zapp React Native Starter App
5. Under React Native Bundle -> Turn off `Allow Caching`
6. On simulator -> Change server type to `Local`
7. On device -> Change server type to `Custom` and in `Custom` field change the IP to your computer's IP running the RN project.
8. Run the app
9. Click on the side menu on the top left (White button - might be hard to see)
10. Select `RN Starter`
11. Shake the phone if on physical device / click `Cmd + d` on the simulator to pop up the debug menu
