# Cordova AdMob Plugin

A free Google AdMob plugin for Cordova.

## Installation

```sh
cordova plugin add cordova-plugin-admob-free --save
```

Since the version 17 of play-services-ads and the 0.21.0 version of the plugin the ADMOB_APP_ID must be added to the AndroidManifest.xml. To install the plugin without errors and to insert the ADMOB_APP_ID to the manifest file automatically use the following code:

```sh
cordova plugin add cordova-plugin-admob-premium --save --variable ADMOB_APP_ID="<YOUR_ADMOB_APP_ID_AS_FOUND_IN_ADMOB>"
```


Note that `cordova plugin add [GIT_URL]` is not supported.

## Usage

### 1. Create Ad Unit ID for your banner and interstitial.

Go to the [AdMob portal](https://www.google.com/admob/) and add your app (if you haven't done so already), once your app is added to your AdMob account, create a new ad unit for it.


### 3. Profit

If you find this plugin useful, please star it.

## Screenshots

| Android Banner                           | Android Interstitial                           |
| ---------------------------------------- | ---------------------------------------------- |
| ![ScreenShot][banner-android-screenshot] | ![ScreenShot][interstitial-android-screenshot] |

| iOS Banner                           | iOS Interstitial                           |
| ------------------------------------ | ------------------------------------------ |
| ![ScreenShot][banner-ios-screenshot] | ![ScreenShot][interstitial-ios-screenshot] |

[banner-android-screenshot]: docs/screenshots/banner-android.jpg
[banner-ios-screenshot]: docs/screenshots/banner-ios.jpg
[interstitial-android-screenshot]: docs/screenshots/interstitial-android.jpg
[interstitial-ios-screenshot]: docs/screenshots/interstitial-ios.jpg

## API

See [documentation page](https://ratson.github.io/cordova-plugin-admob-free/identifiers.html).

## Customize Google Play Services versions (Android only)

The default `PLAY_SERVICES_VERSION` is set to `11.0.4`.
If you need a different version, edit `config.xml` with following,

```xml
<plugin name="cordova-admob-sdk" spec="~0.13.1">
    <variable name="PLAY_SERVICES_VERSION" value="11.6.0" />
</plugin>
```

Note that if you are adding these lines to an existing project, you need to remove both `admob-free` plugin and `android` platform and add them back again to affect the version number.

## Contributing

You can use this Cordova plugin for free unless you are earning a lot.

### Ionic Support

While the Ionic community have provided [an Ionic Native Plugin](https://ionicframework.com/docs/native/admob-free/), plugin users need more examples and tutorials.

As I ([@ratson](https://github.com/ratson)) don't use Ionic myself, it would be great if some experienced Ionic developers could help answering questions or come up with more examples. HELP WANTED HERE.

## Credits

Thanks for the [cordova-plugin-admob-simple](https://github.com/sunnycupertino/cordova-plugin-admob-simple) author for forking the original project [cordova-plugin-admob](https://github.com/floatinghotpot/cordova-plugin-admob) to [make it functional](https://github.com/sunnycupertino/cordova-plugin-admob-simple/issues/1) and open source it.

Screenshots are copied from [cordova-admob-pro](https://github.com/floatinghotpot/cordova-admob-pro).

## Disclaimer

This is NOT an official Google product. It is just a community-driven project, which use the Google AdMob SDKs.

## License

[MIT](LICENSE)
