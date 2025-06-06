<!-- NOTE: THIS FILE IS AUTOGENERATED. DO NOT EDIT BY HAND. -->
<!-- see templates/registry/markdown/attribute_namespace.md.j2 -->

# Android

- [Android Attributes](#android-attributes)
- [Deprecated Android Attributes](#deprecated-android-attributes)

## Android Attributes

The Android platform on which the Android application is running.

| Attribute | Type | Description | Examples | Stability |
|---|---|---|---|---|
| <a id="android-app-state" href="#android-app-state">`android.app.state`</a> | string | This attribute represents the state of the application. [1] | `created` | ![Development](https://img.shields.io/badge/-development-blue) |
| <a id="android-os-api-level" href="#android-os-api-level">`android.os.api_level`</a> | string | Uniquely identifies the framework API revision offered by a version (`os.version`) of the android operating system. More information can be found [here](https://developer.android.com/guide/topics/manifest/uses-sdk-element#ApiLevels). | `33`; `32` | ![Development](https://img.shields.io/badge/-development-blue) |

**[1] `android.app.state`:** The Android lifecycle states are defined in [Activity lifecycle callbacks](https://developer.android.com/guide/components/activities/activity-lifecycle#lc), and from which the `OS identifiers` are derived.

---

`android.app.state` has the following list of well-known values. If one of them applies, then the respective value MUST be used; otherwise, a custom value MAY be used.

| Value  | Description | Stability |
|---|---|---|
| `background` | Any time after Activity.onPause() or, if the app has no Activity, Context.stopService() has been called when the app was in the foreground state. | ![Development](https://img.shields.io/badge/-development-blue) |
| `created` | Any time before Activity.onResume() or, if the app has no Activity, Context.startService() has been called in the app for the first time. | ![Development](https://img.shields.io/badge/-development-blue) |
| `foreground` | Any time after Activity.onResume() or, if the app has no Activity, Context.startService() has been called when the app was in either the created or background states. | ![Development](https://img.shields.io/badge/-development-blue) |

## Deprecated Android Attributes

This document defines attributes that represents an occurrence of a lifecycle transition on the Android platform.

| Attribute | Type | Description | Examples | Stability |
|---|---|---|---|---|
| <a id="android-state" href="#android-state">`android.state`</a> | string | Deprecated. Use `android.app.state` body field instead. | `created`; `background`; `foreground` | ![Deprecated](https://img.shields.io/badge/-deprecated-red)<br>Use `android.app.state` body field instead. |

---

`android.state` has the following list of well-known values. If one of them applies, then the respective value MUST be used; otherwise, a custom value MAY be used.

| Value  | Description | Stability |
|---|---|---|
| `background` | Any time after Activity.onPause() or, if the app has no Activity, Context.stopService() has been called when the app was in the foreground state. | ![Development](https://img.shields.io/badge/-development-blue) |
| `created` | Any time before Activity.onResume() or, if the app has no Activity, Context.startService() has been called in the app for the first time. | ![Development](https://img.shields.io/badge/-development-blue) |
| `foreground` | Any time after Activity.onResume() or, if the app has no Activity, Context.startService() has been called when the app was in either the created or background states. | ![Development](https://img.shields.io/badge/-development-blue) |
