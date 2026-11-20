# KITCHEN GUN — Android app

Ballpoint-pen stickman adventure, packaged as an Android app (runs offline).

## Get the APK
1. Create a new GitHub repository named **kitchen-gun** (account `gnotesamsung7-hue`).
2. Upload everything in this folder (keep the folders, including `.github/workflows`).
3. Open the **Actions** tab — "Build Kitchen Gun APK" runs by itself (about 3–5 minutes).
4. Download `KitchenGun.apk` from **Releases** (or from the finished run under Artifacts).

Direct download link (works once the repo is public and the first build has finished):
https://github.com/gnotesamsung7-hue/kitchen-gun/releases/latest/download/KitchenGun.apk

## Updating the game
Replace `app/src/main/assets/index.html` with the new version, raise `versionCode`
in `app/build.gradle` (1 → 2 → 3...), and push. Every build is signed with the same
key (`app/kitchengun.jks`), so phones update in place and keep saves and drawings.
