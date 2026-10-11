OZORA NAVIGATOR — Android project for GitHub Actions

This is an early test build, not the finished festival app.
It wraps the current HTML prototype in a simple Android WebView and includes a GitHub Actions workflow that builds a debug APK.

How to use:
1. Create a GitHub repository named ozora-navigator.
2. On the repository page choose Add file > Upload files.
3. Extract this ZIP first on a computer if possible, then upload the CONTENTS of this folder (including .github, app, build.gradle, settings.gradle, gradle.properties, README_FIRST.txt). Do not upload the ZIP as a single file.
4. Commit the upload to the main branch.
5. Open the repository's Actions tab. Select "Build Ozora Navigator APK" if prompted, then Run workflow; or let the push-triggered workflow run.
6. When the run completes, open it and download the artifact named Ozora-Navigator-debug-APK. Extract the artifact ZIP to get app-debug.apk.
7. Transfer app-debug.apk to your Samsung A55 and tap it to install. Android may ask you to allow installs from that source.

Current limitations:
- The app is an early prototype. Timetable entries use browser/local WebView storage.
- The current alarm feature is NOT a reliable Android background alarm.
- The GPS feature reports coordinates only; it does not yet route to stages.
- Offline map files are not yet durably stored/calibrated.
- Import selection is not full automatic PDF/image timetable extraction.
- The official Ozora map and verified stage coordinates are not included.
- GitHub Actions builds a debug APK; it is not Play Store-ready or release-signed.
