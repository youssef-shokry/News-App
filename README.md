# News App

<img width="1365" height="768" alt="Gemini_Generated_Image_69gr8b69gr8b69gr" src="https://github.com/user-attachments/assets/1c13789d-f549-46c7-adae-a25e71aec844" />

A Flutter news reader. It pulls articles from a remote news API, shows each one as a card with its image, and opens the full story in the browser.

> Package: `news_c19` · Version 1.0.0+1 · Dart SDK ^3.6.1

* * *

## Features

- Home screen with a greeting and a card for each news category (General, Business, Sports and more), each with a "View All" button.
- A row of news-source tabs (ABC News, Axios and others) to switch where the headlines come from.
- Article cards showing the cover image, headline, author and how long ago it was published.
- Search and side-menu buttons in the top bar.
- Fetches news articles over HTTP using **Dio**.
- Article images load through `cached_network_image`, so a picture downloaded once is served from the cache the next time.
- Publish times show in relative form ("2 hours ago") using `timeago`.
- Tapping an article opens the original story in the device browser through `url_launcher`.
- Material Design UI with local image assets under `assets/images/`.
- Standard Flutter project: Android, iOS, web, Windows, macOS and Linux folders are all present.

* * *

## Tech Stack

| Category        | Technology                                  |
|-----------------|---------------------------------------------|
| Framework       | Flutter (Material Design)                   |
| Language        | Dart ^3.6.1                                 |
| Networking      | `dio` ^5.11.0                               |
| Image caching   | `cached_network_image` ^3.4.1               |
| Date formatting | `timeago` ^3.7.1                            |
| Opening links   | `url_launcher` ^6.3.2                       |
| Icons           | `cupertino_icons` ^1.0.8                    |
| Linting         | `flutter_lints` ^5.0.0                      |

* * *

## Project Structure

```
News-App/
├── android/            # Android platform project
├── ios/                # iOS platform project
├── web/                # Web platform project
├── windows/ macos/ linux/   # Desktop platform projects
├── assets/images/      # local image assets
├── screenshots/        # README images
├── lib/                # Dart source
├── test/               # Flutter tests
├── analysis_options.yaml
└── pubspec.yaml        # dependencies and asset declarations
```

* * *

## Getting Started

### Prerequisites

- Flutter SDK with Dart 3.6.1 or newer (check with `flutter --version`)
- Android Studio or VS Code with the Flutter plugin
- An emulator or physical device (or Chrome, to run the web build)
- An internet connection, since articles are fetched from a remote API

### Build & Run

```
git clone https://github.com/youssef-shokry/News-App.git
cd News-App
flutter pub get
flutter run
```

If the build fails, run `flutter doctor` first. It lists missing SDKs and licenses.

* * *

## Credits

Made by Youssef Ahmed Ali.
