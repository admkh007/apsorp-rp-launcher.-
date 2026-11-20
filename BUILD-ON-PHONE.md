# Build the APK using only your Android phone

This project includes a GitHub Actions cloud build workflow. You do not need Android Studio on your phone.

1. Sign in or create a GitHub account in your phone browser: https://github.com
2. Create a new repository. A public repository is easiest for a first-time setup. Name it `apsorp-rp-launcher`.
3. On the repository page choose **Add file → Upload files**. Extract this ZIP on your phone first, then upload the *contents* of the `APSORP-RP-Launcher` folder (including the hidden `.github` folder and its workflow file). If your file manager hides dot-folders, enable show hidden files.
4. Commit the uploaded files to the `main` branch.
5. Open the repository's **Actions** tab. Select **Build APSORP RP APK**, then **Run workflow** if it has not started automatically.
6. Wait until the workflow shows a green check. Open that run, scroll to **Artifacts**, and download `APSORP-RP-debug-apk`.
7. Extract the downloaded artifact ZIP. It contains `app-debug.apk`. Tap it to install. Android may ask you to allow installs from your browser or file manager.

Important: this produces a debug APK for testing. The launcher currently opens the installed SA-MP Mobile app but has not been proven to pass server IP/port or player name for one-tap auto-connect. You still need to connect inside SA-MP unless its client supports a verified external connect method.
