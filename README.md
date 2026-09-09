# Offclock — Privacy Policy

Public hosting for the Offclock app privacy policy (required by Google Play).

Live page: https://matthewfearne.github.io/offclock-privacy/

The app itself is developed in a separate private repository. This repo contains
only the public-facing privacy policy so it can be served via GitHub Pages.

## Keep this in step with the app

The policy makes specific factual claims. If any of these change in the app, the
policy has to change with it — a privacy policy that overstates how private an
app is, is worse than one that admits a network call.

Current claims that depend on the code:

- **Two permissions are requested from the user:** `POST_NOTIFICATIONS` and
  `RECEIVE_BOOT_COMPLETED`. Adding a third means editing this page.
- **Four more are merged in by Play Billing** and are disclosed: `INTERNET`,
  `ACCESS_NETWORK_STATE`, `com.android.vending.BILLING`, and the generated
  `DYNAMIC_RECEIVER_NOT_EXPORTED_PERMISSION`. Check the built APK, not the
  manifest — `aapt2 dump badging <apk>` is the source of truth, because library
  manifests merge in permissions the app's own manifest never mentions.
- **No Health Connect, no body sensors, no location, no camera.**
- **No analytics, no ads, no third-party trackers.**
- **The only network activity is Google Play Billing**, for the one-time unlock.
  Offclock has no servers of its own. If the app ever gains a backend, sync or
  crash reporting, this page must be updated *before* that release ships.
