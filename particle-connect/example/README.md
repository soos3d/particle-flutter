# particle_connect_example

An example Flutter application demonstrating how to integrate and use the `particle_connect` plugin for wallet connection and user onboarding.

## Prerequisites

Before running this example, obtain your **Project ID**, **Client Key**, and **App ID** from the [Particle Network Dashboard](https://dashboard.particle.network/).

## Configuration

1. Add your credentials to `android/app/build.gradle`:

    ```gradle
    manifestPlaceholders["PN_PROJECT_ID"] = "YOUR_PROJECT_ID"
    manifestPlaceholders["PN_PROJECT_CLIENT_KEY"] = "YOUR_CLIENT_KEY"
    manifestPlaceholders["PN_APP_ID"] = "YOUR_APP_ID"
    ```

2. Add your credentials to `lib/connect_demo/connect_logic.dart`:

    ```dart
    const projectId = "YOUR_PROJECT_ID";
    const clientK = "YOUR_CLIENT_KEY";
    ```

## Running

```sh
flutter run
```
