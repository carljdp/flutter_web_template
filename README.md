# flutter_web_template [#](https://github.com/carljdp/flutter_web_template)

Flutter Web Template

## Pre-requisites

- NVM / NodeJS
- Flutter / Dart / Android Studio
- VSCode (with Flutter and Dart extensions)

## Dev Guide

Commands used to create this project:

Showing explicit options (even if they are default) to avoid any confusion.

```bash

flutter channel stable

flutter upgrade

flutter create flutter_web_template  --description "Flutter Web Template" --org "za.web.tech" --project-name "flutter_web_template" --platforms "web" --template=app --empty --disable-telemetry

cd flutter_web_template

flutter config --build-dir=build/ --enable-web --no-enable-linux-desktop --no-enable-macos-desktop --no-enable-windows-desktop --no-single-widget-reload-optimization --no-enable-android --no-enable-ios --no-enable-fuchsia --no-enable-custom-devices --no-analytics

flutter pub get

flutter run --debug --hot --web-hostname=127.0.0.1 --web-port=8080 --device-id=edge --web-renderer=html --no-web-resources-cdn

```

And then to build the release version:

(But this has not yet been refined)

```bash

# ensure the .env file exists

flutter build web --dart-define-from-file=.env --pub --release --base-href=/ --web-renderer=html

```

---

Author: [Carl J du Preez](https://linktr.ee/CarlJdP)

[License](https://github.com/carljdp/flutter_web_template/blob/master/LICENSE)
