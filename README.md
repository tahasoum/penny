# Penny — build your Android APK (free, no Android Studio)

This folder builds a real Android APK for you using GitHub's free servers.
You don't install anything. You just upload these files and download the APK.

## Steps (about 10 minutes, mostly waiting)

1. Make a free account at https://github.com (skip if you have one).

2. Click the "+" top-right → "New repository".
   - Name it: penny
   - Set it to Public (free build minutes) or Private (also fine)
   - Click "Create repository".

3. On the new repo page, click "uploading an existing file".
   - Drag in EVERYTHING from this folder:
       config.xml
       package.json
       www/  (the folder, with index.html inside)
       .github/  (the folder, with the workflow inside)
   - Important: keep the folder structure. The .github folder must stay named .github
   - Click "Commit changes".

4. GitHub now builds the APK automatically.
   - Click the "Actions" tab at the top.
   - You'll see "Build Penny APK" running (yellow dot). Wait until it turns green (~3-5 min).

5. Download your app.
   - Click the finished green run.
   - Scroll to "Artifacts" at the bottom → click "penny-apk" to download a zip.
   - Inside is app-debug.apk — that's your app.

6. Install on your phone.
   - Copy the .apk to your Android phone.
   - Tap it → allow "Install from unknown sources" if asked → Install.
   - Penny is now a real installed app. All data stays on your phone.

## Notes
- This produces a DEBUG apk — perfect for personal use and installing on your own phone.
- A "release" apk (for the Play Store) needs a signing key; ask and I'll add those steps.
- To update the app later: change www/index.html in the repo, and a fresh APK builds automatically.
