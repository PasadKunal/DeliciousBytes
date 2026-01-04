DeliciousBytes
=================

A delightful Flutter food-delivery prototype showcasing product lists, cart functionality, and simple state management. Built as a learning/demo app and ready to be customized for your portfolio or store submission.

Highlights
- Clean Flutter UI with pages for popular and recommended food
- Cart with history and controllers for state management
- Localized strings in `assets/language` (English + Arabic)
- Ready for Android and iOS builds


Tech stack
- Flutter & Dart
- Basic REST client for product data under `lib/data/api`


Prerequisites
- Install Flutter: https://flutter.dev/docs/get-started/install
- Ensure Android SDK / Xcode are installed for respective platforms


Clone and run

```bash
git clone "https://github.com/PasadKunal/DeliciousBytes.git"
cd "DeliciousBytes"
flutter pub get
flutter run
```


Run on specific device/emulator

```bash
flutter devices
flutter run -d <device-id>
```


Run tests

```bash
flutter test
```


Project structure (important files)
- [pubspec.yaml](pubspec.yaml) — app metadata, assets & dependencies
- [lib/main.dart](lib/main.dart) — app entry point
- [lib/pages](lib/pages) — UI pages
- [lib/controllers](lib/base/controllers) — app controllers (state)
- [lib/data/api](lib/data/api) — API client and repository code
- [assets/language](assets/language) — translations


Publishing checklist (quick)
- Run `flutter build apk` or `flutter build appbundle` for Play Store
- Run `flutter build ios` and archive via Xcode for App Store


Development notes
- The app uses simple controller classes under `lib/base/controllers` that manage cart and products. Look at `cart_controller.dart` and `popular_product_controller.dart` to understand data flow.
- API client and repository pattern: `lib/data/api/api_client.dart` and repos under `lib/data/repository`.

