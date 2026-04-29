# Hitron Wi-Fi Installation Universal Link

This folder is intended to be deployed at the root of the GitHub Pages user site:

```text
https://rheasue.github.io/
```

The QR code should point to:

```text
https://rheasue.github.io/app.installation/
```

## Required iOS Configuration

The app entitlements must contain:

```text
applinks:rheasue.github.io
```

The AASA file contains these app IDs:

```text
X9Q52CSADY.com.hitrontech.myhitroncloud
98AMPRY4QV.com.hitrontech.szrd.fizz.wifi
98AMPRY4QV.com.hitrontech.szrd.midco
```

## Deploy

1. Create or open the GitHub Pages user repository named `rheasue.github.io`.
2. Put every file in this folder at the repository root.
3. Enable GitHub Pages for the repository.
4. Confirm these URLs are reachable:

```text
https://rheasue.github.io/.well-known/apple-app-site-association
https://rheasue.github.io/app.installation/
```

## Production Notes

Replace the App Store search URLs in `app.installation/index.html` with the final App Store links for MyHitron+, Fizz Wi-Fi, and Freestyle.

After installing a build with the updated entitlements, delete and reinstall the app on the test phone to force iOS to refresh Universal Link association.
