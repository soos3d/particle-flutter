# Social Login with Account Abstraction Guide

A Flutter guide application demonstrating how to combine social login with Account Abstraction using [Particle Network](https://particle.network)'s SDKs.

This guide covers setting up social authentication alongside ERC-4337 Account Abstraction, enabling gasless transactions and smart account features for socially authenticated users.

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
- [AA Flutter Doc](https://developers.particle.network/api-reference/aa/sdks/mobile/flutter)
