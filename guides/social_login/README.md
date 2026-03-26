# Social Login Guide

A Flutter guide application demonstrating how to implement social login using [Particle Network](https://particle.network)'s Auth Core SDK.

This guide covers setting up social authentication (Google, Apple, Twitter, etc.) in a Flutter app using `particle_auth_core` and `particle_connect`.

## Prerequisites

Before running this guide, obtain your **Project ID**, **Client Key**, and **App ID** from the [Particle Network Dashboard](https://dashboard.particle.network/).

## Configuration

1. Add your credentials to `android/app/build.gradle`:

    ```gradle
    manifestPlaceholders["PN_PROJECT_ID"] = "YOUR_PROJECT_ID"
    manifestPlaceholders["PN_PROJECT_CLIENT_KEY"] = "YOUR_CLIENT_KEY"
    manifestPlaceholders["PN_APP_ID"] = "YOUR_APP_ID"
    ```

2. Add your credentials to the relevant Dart initialization file in `lib/`.

## Running

```sh
flutter run
```

## Related Documentation

- [Auth Core Flutter Doc](https://developers.particle.network/api-reference/auth/mobile-sdks/flutter)
- [Connect Flutter Doc](https://developers.particle.network/api-reference/connect/mobile/flutter)
