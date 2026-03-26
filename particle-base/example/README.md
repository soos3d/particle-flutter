# particle_base_example

An example Flutter application demonstrating the shared base utilities provided by the `particle_base` plugin.

## Prerequisites

Before running this example, obtain your **Project ID**, **Client Key**, and **App ID** from the [Particle Network Dashboard](https://dashboard.particle.network/).

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
