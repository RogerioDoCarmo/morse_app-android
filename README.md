# morse_app-android

**Auto-generated build mirror. Do not edit directly — changes will be overwritten.**

This repository holds a buildable snapshot of the Android/Gradle project for
[OmniMorse](https://github.com/RogerioDoCarmo/morse_app), regenerated
automatically whenever a new release is published in the main repo.

It exists to give F-Droid (and any other build system that wants a plain
Gradle project) a source tree that builds with standard tools: the generated
`android/` project (output of `expo prebuild`) is committed here, dependencies
are installed at build time with `pnpm install --frozen-lockfile` (pinned by
the committed `pnpm-lock.yaml`), and `.npmrc` sets `node-linker=hoisted` so
`node_modules` comes out flat and symlink-free — required for F-Droid's
source scanner, which resolves real paths.

The committed `package.json` sets Expo's autolinking option
`buildFromSource: [".*"]`, so every Expo/React Native native module is
compiled from source by Gradle instead of consuming the prebuilt AARs that
Expo ships.

**This is the F-Droid build, not the store build.** It is prebuilt with
`OMNIMORSE_BUILD_VARIANT=fdroid`, which leaves out Firebase Crashlytics and
`expo-updates`, patches Google's ML Kit out of `expo-camera` and the Play
Install Referrer out of `expo-application`, and drops the `INTERNET`
permission. What each build includes, and why, is in
[`notes/FDROID.md`](https://github.com/RogerioDoCarmo/morse_app/blob/develop/notes/FDROID.md).

- **App source, issues, and development:** [RogerioDoCarmo/morse_app](https://github.com/RogerioDoCarmo/morse_app)
- **License:** MIT (same as the source repo)
- **Updated by:** [`.github/workflows/android-mirror.yml`](https://github.com/RogerioDoCarmo/morse_app/blob/develop/.github/workflows/android-mirror.yml) in the main repo, on every GitHub release.
- **F-Droid store metadata:** `fastlane/metadata/android/<locale>/`, generated
  from the main repo's store listing on every mirror run.

Each push here is tagged with the version of the corresponding morse_app
release (e.g. `v0.3.7`).
