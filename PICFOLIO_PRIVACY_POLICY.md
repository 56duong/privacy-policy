# Privacy Policy for Picfolio

**Last updated:** October 2026

## Overview

Picfolio is a photo organizer app. Unlike most apps, **Picfolio has no server of its own and does not collect, store, or have access to any of your data.** Instead, Picfolio connects directly from your device to your own private GitHub repository using a GitHub access token that you provide. Your photos live in that repository, under your full control — not on any server operated by the developer of this app.

This policy explains exactly what Picfolio accesses on your device, where things are stored, and what Picfolio deliberately does *not* do.

## What Picfolio accesses, and why

- **GitHub access token** — the token you generate and paste into the app. It is encrypted on your device using the Android Keystore (`EncryptedSharedPreferences`) and is used only to make requests directly from your device to GitHub's own API over HTTPS. It is never sent anywhere other than GitHub, and it is never visible to the developer of this app.
- **Your photos** — stored in the private GitHub repository you connect. Picfolio uploads, downloads, and organizes files in that repository on your behalf, directly between your device and GitHub. The developer of this app has no access to your repository or its contents.
- **Camera** — used only if you choose to take a photo from within the app, to upload it.
- **Photos/media on your device** — used only to let you pick existing photos to upload, and to save photos you choose to download back to your device's gallery.
- **Biometric hardware (fingerprint/face), if you enable App Lock** — authentication is handled entirely by Android's own BiometricPrompt system. Picfolio never receives or stores your fingerprint or face data; it only receives a yes/no result from the operating system.
- **PIN, if you set one for App Lock** — stored on your device only, as a salted cryptographic hash (never the PIN itself), and is never transmitted anywhere.
- **Internet access** — used solely to communicate with GitHub's API (`api.github.com`) and, if you follow links from the in-app GitHub setup guide, to open GitHub's website in your browser.

## What Picfolio does not do

- No server. There is no backend operated by this app's developer, and therefore no central database of user data anywhere outside your own device and your own GitHub repository.
- No advertising network of any kind.
- No analytics or tracking SDKs.
- No account system of its own — you authenticate directly with GitHub using your own token.
- Picfolio does not sell, share, or transmit your data to any third party, because it never has access to it in the first place.

## Third-party service: GitHub

Picfolio communicates directly with GitHub's REST API to store and retrieve your photos and folder data. This means your use of Picfolio is also subject to [GitHub's own Privacy Statement](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement) and [Terms of Service](https://docs.github.com/en/site-policy/github-terms/github-terms-of-service), since GitHub, Inc. (a subsidiary of Microsoft) independently processes data you send through their API as part of operating your repository.

## Where your data lives

- **On your device:** your encrypted GitHub token, an encrypted App Lock PIN (if set), and a local cache of folder/photo listings and captions used to make the app load instantly and avoid unnecessary network requests. Uninstalling Picfolio permanently deletes all of this.
- **On GitHub:** your photos, folder structure, captions, and favorites metadata, stored in the private repository you created and connected. This is entirely separate from the app and is **not affected by uninstalling Picfolio** — your repository and its contents remain exactly as they are on GitHub, under your ownership, unless you delete them yourself through GitHub directly.

## Permissions this app requests

| Permission | Purpose |
|---|---|
| Camera | Only used if you take a photo within the app to upload it. |
| Photos / Media | Used to select photos to upload, and to save photos you download. |
| Internet | Used to communicate with GitHub's API. |
| Biometric / Fingerprint | Only used if you enable the optional App Lock feature. |

## Children's privacy

Picfolio is not directed at children and does not knowingly collect any data from children under 13. Since the app has no server and collects no data on its own, there is no mechanism by which it could do so.

## Changes to this policy

This policy may be updated from time to time, for example if new features change what the app accesses. The "Last updated" date at the top will reflect the most recent revision. Continued use of the app after a change constitutes acceptance of the updated policy.

## Contact

Questions about this policy or the app can be sent to: **56duong@gmail.com**
