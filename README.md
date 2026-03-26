# Particle Flutter SDKs

![pub version](https://img.shields.io/pub/v/particle_base?color=blue&style=round)

<img width="420" src="/images/connectkit-mobile.svg">

A collection of Flutter plugins for integrating Particle Network's authentication, wallet connection, embedded wallet, and account abstraction features into mobile apps.

## Packages

| Package | Description | Docs |
|---|---|---|
| `particle_auth_core` | Self-custodial authentication infrastructure for Web3 apps and wallets | [Auth Core Doc](https://developers.particle.network/api-reference/auth/mobile-sdks/flutter) |
| `particle_connect` | Wallet connection and user onboarding for dApps | [Connect Doc](https://developers.particle.network/api-reference/connect/mobile/flutter) |
| `particle_wallet` | Embedded wallet infrastructure for apps and wallets | [Wallet Doc](https://developers.particle.network/api-reference/connect/mobile/flutter) |
| `particle_aa` | Account Abstraction support | [AA Doc](https://developers.particle.network/api-reference/aa/sdks/mobile/flutter) |
| `particle_base` | Shared base utilities used by all Particle plugins | — |

## Upgrade Guide

If you are upgrading from 1.4.x, please review the [Upgrade Guide](https://github.com/Particle-Network/particle-flutter/blob/master/UpgradeGuide.md) before proceeding.

## iOS Notes

`particle_auth_core` supports **ios-arm64 (physical devices) only** — iOS simulators are not supported. Testing requires an actual iPhone device.

When using CocoaPods on iOS, pin all pod versions in your `Podfile`. Refer to the native iOS repositories for the latest versions: [particle-ios](https://github.com/Particle-Network/particle-ios) and [particle-connect-ios](https://github.com/Particle-Network/particle-connect-ios).

## Installation

Add the packages you need to your Flutter project:

```sh
flutter pub add particle_auth_core
flutter pub add particle_connect
flutter pub add particle_wallet
flutter pub add particle_aa
```

Then import them in your Dart code:

```dart
import 'package:particle_auth_core/particle_auth_core.dart';
import 'package:particle_connect/particle_connect.dart';
import 'package:particle_wallet/particle_wallet.dart';
import 'package:particle_aa/particle_aa.dart';
```

## Running the Example

1. Navigate to the `particle-connect/example` directory.
2. Obtain your **Project ID**, **Client Key**, and **App ID** from the [Particle Network Dashboard](https://dashboard.particle.network/).
3. Add your credentials to `particle-connect/example/android/app/build.gradle`:

    ```gradle
    manifestPlaceholders["PN_PROJECT_ID"] = "YOUR_PROJECT_ID"
    manifestPlaceholders["PN_PROJECT_CLIENT_KEY"] = "YOUR_CLIENT_KEY"
    manifestPlaceholders["PN_APP_ID"] = "YOUR_APP_ID"
    ```

4. Add your credentials to `particle-connect/example/lib/connect_demo/connect_logic.dart`:

    ```dart
    const projectId = "YOUR_PROJECT_ID";
    const clientK = "YOUR_CLIENT_KEY";
    ```

5. Run the app:

    ```sh
    flutter run
    ```

For transaction structuring examples (including contract reads and writes), see `particle-auth/example/lib/mock/transaction_mock.dart`.
