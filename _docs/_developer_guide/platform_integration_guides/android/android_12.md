---
nav_title: Android 12 Upgrade Guide
page_order: 9
platform: Android
description: "This reference article covers the Android 12 SDK update, highlighting changes such as deep linking, SDK compatibility, and more."
---

# Android 12 SDK Upgrade Guide

This guide describes relevant changes introduced in Android 12 (2021) and the required upgrade steps for your Braze Android SDK integration.

For a full migration guide of Android 12, see the [Android Developer Documentation](https://developer.android.com/about/versions/12).

{% alert info %}
In previous testing of Android 12 betas, we identified an issue which would have required upgrading the Braze Android SDK regardless of your app's Target version. This has since been corrected in the latest Android Beta, and an upgrade is no longer required.
{% endalert %}

## Braze SDK Compatibility

The following changes are only required when your app is targeting Android 12.

**What happens if I don’t upgrade my Braze Android SDK?**

* Changes in [component exports](https://developer.android.com/about/versions/12/behavior-changes-12#exported), [pending intents](https://developer.android.com/about/versions/12/behavior-changes-12#pending-intent-mutability), [notification trampolines](https://developer.android.com/about/versions/12/behavior-changes-12#notification-trampolines) may impact your ability to compile your app, or may prevent the Braze SDK from initializing. This behavior occurs only for apps targeting Android 12.
* Changes in [custom push notifications](https://developer.android.com/about/versions/12/behavior-changes-12#custom-notifications) have changed the layout for our new [Android Inline Image Push](https://www.braze.com/docs/developer_guide/platform_integration_guides/android/push_notifications/inline_image_push/) feature. This behavior occurs only for apps targeting Android 12.

[1]: https://github.com/Appboy/appboy-android-sdk/blob/master/CHANGELOG.md#1312
