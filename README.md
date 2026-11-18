# Reverse Launcher

Reverse Launcher is a TV-first Android home launcher. This public repository contains user-facing release information and signed APKs; the application source code is not published here.

## Download and install

Download the signed APK from the [latest release](https://github.com/abnazroy/reverselauncher-releases/releases/latest), then open it on your Android TV or phone and follow Android's installation prompts. If Android asks, allow the file manager or browser you used to install apps. Select Reverse Launcher as the Home app when prompted.

## Enable Home redirect

In Reverse Launcher, open **Settings > Access Permissions > Make default home**. In Android TV Settings, open **Accessibility** and enable both the system Accessibility switch and **Reverse Launcher home redirect**. Both must be active for Home redirect to work. Some TVs leave the service selected while system Accessibility is off; if Reverse Launcher reports **System off**, enable the system switch as well. The service only detects supported TV Home launcher windows and cannot read screen content.

## Enable Continue Watching

On Android TV, open **Settings > Apps > Special app access > Notification access** (sometimes called **Notification listener access**) > **Reverse Launcher** > **Allow**.

This special access is different from **Settings > Apps > Reverse Launcher > Notifications**. The app-info Notifications switch controls notifications shown by the launcher; Notification Access allows Continue Watching to read media-session details from supported apps. Some TV firmware does not expose a direct settings shortcut, so use the manual path above.

## Enable Home redirect

Home redirect requires Android's system Accessibility switch and the Reverse Launcher service to both be active. A TV can still list the service while system Accessibility is off; in that state, Home redirect will not run.

## Find Special App Permissions on Older Android TVs

Settings names and locations vary by Android version and TV manufacturer. These are common paths, not guarantees.

- **Android TV 8 (Oreo) and newer:** Android uses a per-app **Install unknown apps** permission. On many Android TV 9, 10, and 11 devices, find it under **Settings > Apps > Special app access**. This area may also contain **Display over other apps**, **Usage access**, and **Notification access**. Select the app that needs access; for sideloading, allow only the browser or file manager you use to open the APK.
- **Android 7.1.1 and older:** These versions typically use a global **Unknown sources** switch under **Settings > Security** or **Security & restrictions**. Enable it only when needed and turn it off afterward.
- **If a setting is missing:** TV firmware may rename, move, or omit settings. Some TVs expose Developer options under **Settings > Device Preferences** (or **System**) > **About** after selecting **Build** or **Build number** seven times. This reveals developer options, but does not guarantee that a missing special-access setting is available.

### Compared with Google TV

Google TV and Android TV share the Android platform, but menu paths and available controls vary by OS version, device manufacturer, and firmware. Newer privacy, profile, and family controls are not available uniformly on older Android TVs. For sideloading, Android 8.0 and newer use per-app install-source permission; Android 7.1.1 and older use the global **Unknown sources** setting.

Reference: [Android Developers - Install unknown apps](https://developer.android.com/distribute/marketing-tools/alternative-distribution#unknown-sources).

## Screenshots

![Home screen with fern canopy wallpaper](screenshots/01-home-fern-canopy.png)

![Launcher settings](screenshots/02-settings.png)

![Home screen with neon city wallpaper](screenshots/04-home-neon-city.png)

![TV access permissions for Home redirect and Continue Watching](screenshots/06-access-permissions.png)

## Support the Developer

Reverse Launcher is free to use, with no ads, subscriptions, or paid features. Optional donations help support development, device testing, and maintenance; donating does not unlock features.

If Reverse Launcher is useful to you, [donate to Reverse Launcher](https://www.paypal.com/ncp/payment/RX34HJHT2TPF8).

## Releases

See the [release history](https://github.com/abnazroy/reverselauncher-releases/releases) for APK downloads and version notes.
