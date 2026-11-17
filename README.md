# HyFlix Remote Control & In-App Update API

This repository contains the dynamic remote configuration JSON for the **HyFlix (Sahitya Stream)** mobile application.

### Raw JSON Endpoint:
`https://raw.githubusercontent.com/skhub-tech/hyflix_update/main/app_config.json`

### Controls Available:
- **`app_update`**:
  - `version_code`: Set higher than installed app version code to trigger update dialog.
  - `version_name`: Display version string (e.g. `1.0.1`).
  - `title`: Update dialog headline.
  - `description`: Multiline changelog features.
  - `download_url`: Direct APK download link or release page.
  - `button_text`: Primary action button label.
  - `force_update`: `true` forces immediate update without dismiss option; `false` allows user to tap "Later".
- **`adsterra_monetization`**:
  - `enabled`: `true` to require sponsor visit before download, `false` to disable ads.
  - `direct_link`: Your Adsterra Smartlink URL.
  - `unlock_hours`: Hours the download remains unlocked after one sponsor visit (default 24h).
