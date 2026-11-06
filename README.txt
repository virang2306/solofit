SOLOFIT AS A REAL ANDROID APP (private, no website, no laptop running)
=====================================================================
You need: a free GitHub account and a laptop/PC for about 10 minutes (one time only).

1. Go to github.com and sign up (free). Then click New repository.
   Name it solofit, choose PRIVATE (only you can see it), click Create repository.
2. On the new repository page click "uploading an existing file".
3. Open this SoloFit-App folder. Select EVERYTHING inside it
   (package.json, capacitor.config.json, www, .github, README.txt)
   and drag it into the GitHub page. Click Commit changes.
   - If the .github folder did not upload: click Add file > Create new file, type
     .github/workflows/android.yml as the name, paste the contents of that file, Commit.
4. Click the Actions tab (click "enable" if it asks). The "Build APK" job starts by itself.
   Wait 5 to 10 minutes until it shows a green tick. If it shows a red cross, open it and
   send me a screenshot of the error.
5. Click the finished run. At the bottom, under Artifacts, download SoloFit-APK.
   Unzip it. Inside is app-debug.apk.
6. Send app-debug.apk to your phone (WhatsApp to yourself, Drive or USB), open it and
   allow "Install unknown apps" when asked. SoloFit is now a normal app with an icon.

To update later: replace www/index.html in the repository and the APK is rebuilt.

NOTES
- Your progress is saved inside the app on the phone. Use Log > Copy backup now and then.
- This first version has the default app icon and in-app reminders (same as the web version).
  Background reminders and the phone step sensor need extra native plugins, which come next.
