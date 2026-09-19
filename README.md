<div align=center>

# Droidík
###### a tiny APK runtime aiming to make the Android experience of running APKs on your system seem seamless and integrated into the whole OS

</div>

Droidík is a small desktop tool for running Android apps without dealing with a full Android emulator UI. The idea is simple: give Droidík an APK, and it starts a lightweight Android environment in the background and opens the app in its own window.

## Why?

Most Android emulators are built around pretending that your computer is an Android tablet or phone. That's overkill if you just want to run an app. Droidík aims to make Android apps feel more like normal desktop applications.

Eventually, using it should be as simple as:

```bash
droidik app.apk
```

or just double-clicking an APK.

## How it works

Droidík is not a new Android emulator. Instead, it uses an existing Android runtime/emulator underneath and handles the annoying parts for you:

* starting Android in the background
* installing the APK
* launching the correct activity
* showing the app in a normal desktop window
* shutting everything down when you're done

The Android system itself should mostly stay out of sight.

## Goals

* Simple APK launching
* No Android Studio required
* No Android launcher or phone-like UI
* Fast startup using snapshots
* ARM64 support, especially on Apple Silicon
* Windows and macOS support
* Minimal configuration
* Support for split APKs / `.apks` later

## Status

Experimental. Right now this is mostly an idea. The first version will likely be a thin wrapper around an existing Android emulator, ADB and a desktop display layer.

## Name

**Droidík** is basically a tiny droid.

The project name uses the Czech `í`, but the CLI command and package names use plain ASCII:

```bash
droidik
```

