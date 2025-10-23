InMobi SDK for Android
======================

Modified: 23 October, 2025

SDK Version: 11.0.0

Thanks for monetizing with InMobi!
If you haven't already, [sign up](https://www.inmobi.com/user/index?locale=en_us#signup) for an account to start monetizing your app!

## Download
The InMobi SDK for Android is available via:

**mavenCentral AAR**

The InMobi SDK is available as a AAR via mavenCentral; to use it, add the following to your `build.gradle`

```
repositories {
    mavenCentral()
}
dependencies {
    implementation 'com.inmobi.monetization:inmobi-ads-kotlin:11.0.0'
}
```

**Download from the support portal**

To download the latest SDK as a AAR, please visit [http://inmobi.com/sdk](https://inmobi.com/sdk).

**To continue integrating with the InMobi SDK, please see the [Integration Guidelines](https://support.inmobi.com/monetize/android-guidelines/) for Android.**

## New in this version
    • Upgraded support for native ads
    • Bug Fixes and Enhancements
    • APIs Removed
        InMobiNative
            - public String getAdIconUrl()
            - public String getAdLandingPageUrl()
            - public boolean isAppDownload()
            - public JSONObject getCustomAdContent()
            - public View getPrimaryViewOfWidth(Context context, View convertView, ViewGroup parent, int viewWidthInPixels)
            - public void reportAdClickAndOpenLandingPage()
        NativeAdEventListener
            - public void onAdReceived(@NonNull InMobiNative ad)
            - public void onAdFullScreenWillDisplay(@NonNull InMobiNative ad)
            - public void onAdImpressed(@NonNull InMobiNative ad)
            - public void onAdStatusChanged(@NonNull InMobiNative nativeAd)

    • APIs Added
        New Class Added : InMobiNativeImage
        New Class Added : InMobiNativeViewData
        New Class Added : MediaView
        InMobiNative
            - public InMobiNativeImage getAdIcon()
            - public String getAdvertiserName()
            - public View getAdChoiceIcon()
            - public void registerViewForTracking(InMobiNativeViewData viewData)
            - public void unTrackViews()
            - public MediaView getMediaView()
            - public boolean isVideo()
            - public String getCreativeId()
            - public JSONObject getAdContent()

** Refer to [Release Notes](https://support.inmobi.com/monetize/sdk-documentation/android-guidelines/changelogs-android) for Older Versions.**

## Requirements
- Android 4.4 (API level 19) and higher
- androidx.appcompat (Not a dependency of SDK. Used only in Sample App)

## License
To view the license for the InMobi SDK, see [here](https://github.com/InMobi/sdk-sample-code-android/blob/master/sdk/licenses/License.txt). To view the terms of service, visit [https://inmobi.com/terms-of-service](http://inmobi.com/terms-of-service/).
The code for the sample apps is provided under the Apache 2.0 License.

