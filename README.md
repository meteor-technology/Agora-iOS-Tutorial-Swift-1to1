# iOS 1-to-1 Tutorial for Swift

This tutorial enables you to quickly get started in your development efforts to create an iOS app with real-time video calls, voice calls, and interactive broadcasting. With this sample app you can:

**This repository is fork from [AgoraIO/Basic-Video-Call](https://github.com/AgoraIO/Basic-Video-Call).**

- Start and end audio/visual communication between two users.
- Join a communication channel.
- Mute and unmute audio.
- Enable and disable video.
- Switch between the front and rear cameras.

## Prerequisites

- Xcode 11+
- Physical iOS device (iPhone or iPad)

## Quick Start

This section shows you how to prepare, build, and run the sample application.

### Obtain an App ID

To build and run the sample application, get an App ID:
1. Create a developer account at [agora.io](https://dashboard.agora.io/signin/). Once you finish the signup process, you will be redirected to the Dashboard.
2. Navigate in the Dashboard tree on the left to **Projects** > **Project List**.
3. Save the **App ID** from the Dashboard for later use.
4. Generate a temp **Access Token** (valid for 24 hours) from dashboard page with given channel name, save for later use.

5. Open `Agora iOS Tutorial.xcodeproj` and edit the `AppID.swift` file. In the `agoraKit` declaration, update `<#Your App Id#>` with your app ID, and assign the token variable with the temp Access Token generated from dashboard.

    ``` Swift
    let AppID: String = <#Your App ID#>
    // assign Token to nil if you have not enabled app certificate
    let Token: String? = <#Temp Token#>
    ```

### Integrate the Agora Video SDK
- Install Agora Video SDK with CocoaPods. e.g. `bundle exec pod install`
- open `Agora iOS Tutorial.xcworkspace`

## Resources

- You can find full API document at [Document Center](https://docs.agora.io/en/)
- You can file bugs about this demo at [issue](https://github.com/AgoraIO/Basic-Video-Call/issues)

## License

The MIT License (MIT)
