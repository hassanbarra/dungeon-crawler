# Get the APK with no computer setup (free GitHub account)

1. Create a free account at github.com and tap **New repository** (name it `dungeon-crawler`, Public or Private).
2. Unzip `dungeon-crawler.zip`. On the repo page choose **Add file > Upload files** and drag in EVERYTHING inside the unzipped folder (client, shared, scripts, package.json ...).
3. Hidden folders are often skipped by uploads. So also tap **Add file > Create new file**, type the name `.github/workflows/build-apk.yml`, paste the contents of `build-apk.yml` (included next to the zip), and tap **Commit changes**.
4. Open the **Actions** tab. If asked, enable workflows. Pick **Build APK**, tap **Run workflow**. (Committing also starts it.)
5. Wait ~10-15 minutes. Open the finished run, scroll to **Artifacts**, download **DungeonCrawler-apk** (a zip containing `DungeonCrawler.apk`).
6. Copy the APK to each phone and install it. See PLAY.md for how to host and join.

If the run fails (red X), open it, copy the error text from the failed step, and paste it to me.
