# AdColony iOS SDK
* Modified: August 3rd, 2021
* SDK Version: 4.7.0

## Overview

AdColony delivers zero-buffering,
[full-screen Instant-Play™ HD video](https://www.adcolony.com/technology/instant-play/),
[interactive Aurora™ Video](https://www.adcolony.com/technology/auroravideo),
and Aurora™ Playable ads that can be displayed anywhere within your
application. Our advertising SDK is trusted by the world’s top gaming
and non-gaming publishers, delivering them the highest monetization
opportunities from brand and performance advertisers. AdColony’s SDK
can monetize a wide range of ad formats including in-stream/pre-roll,
out-stream/interstitial and V4VC™, a secure system for rewarding users
of your app with virtual currency upon the completion of video and
playable ads.

## Release Notes

### 4.7.0

* Internal communication adjustments to improve CPU usage and battery life
* Additional ad request safety to avoid potential timeouts
* Fixed issue where interstitial ad show attempts would fail without feedback when a network filter mismatch occurred
* Optimized data returned via collectSignals()
* Fixed edge case ad playback issues due to SKStoreProductController
* Internal file directory refactoring to reach parity with Android behavior
* Fixed race condition where asynchronous collectSignals() would return an empty String
* Removed public block interface and native ad view API
* Mac M1 emulator support
* Various other bug fixes and performance improvements

Here is the link to the
[release notes](https://github.com/AdColony/AdColony-iOS-SDK/blob/master/CHANGELOG.md)
for all the previous SDK versions.

## Getting Started

To get started, here is the link to
[iOS SDK integration documentation](https://github.com/AdColony/AdColony-iOS-SDK/wiki).

**Note:**

Per Apple's direction, we have built our latest SDK against its iOS 14.5 release candidate (RC) as distributed to iOS developers on April 20th, 2021, and recommend all of our iOS publishing partners build against this release. Additionally, per Apple's documentation, ensure apps are submitted against the iOS 14.5 RC version, and built using Xcode 12.5 Release Candidate. Beginning Starting April 26, 2021, all iPhone and iPad apps submitted to the App Store must be built with Xcode 12 and the iOS 14 SDK or later. For further questions, please contact your AdColony Monetization Manager, or email support@adcolony.com.

* Tested and verified on iOS 14.5
* Xcode 12.5 and up
* Works on iOS 9 and above.
* Not backwards compatible with any AdColony 2.0 integrations due to major API changes.

## Upgrading

#### SDK 2.X

Please note that updating from our 2.x SDK is not a drag and drop
update, but rather includes breaking API and process changes. In order
to take advantage of the 3.x SDK, a complete re-integration is
necessary. Please review our
[documentation](https://github.com/AdColony/AdColony-iOS-SDK/wiki)
to get a better idea on what changes will be necessary in your app.

For detailed information about the AdColony SDK, see our
[iOS SDK documentation](https://github.com/AdColony/AdColony-iOS-SDK/wiki).

#### SDK 3.X

Updating from 3.x SDK is still drag and drop update although you'll see deprecation warnings on interstitial API.
3.x interstitial API is still fully functional and will remain fully functional at least until iOS 14 release.
Just drag and drop the framework into your Xcode project. If you are
using Cocoapods, sync with the latest by running `pod update`.

For detailed information about the AdColony SDK, see our
[iOS SDK documentation](https://github.com/AdColony/AdColony-iOS-SDK/wiki).



## Legal Requirements

By downloading the AdColony SDK, you are granted a limited,
non-commercial license to use and review the SDK solely for evaluation
purposes.  If you wish to integrate the SDK into any commercial
applications, you must register an account with AdColony and accept
the terms and conditions on the AdColony website.

Note that U.S. based companies will need to complete the W-9 form and
send it to us before publisher payments can be issued.

## Contact Us

For more information, please visit AdColony.com. For questions or
assistance, please email us at support@adcolony.com.
