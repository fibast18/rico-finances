MY FINANCES v1.7.5 — COMPACT HEADER LAYOUT (CUMULATIVE OFFLINE EDITION)
============================================================================

NEW IN v1.7.5
- Aligns My Finances title horizontally with the AI and Settings buttons in the FIRST row.
- Keeps the personalized greeting directly underneath.
- Aligns the live, localized weekday/date with the ONLINE/OFFLINE badge in the LAST row.
- Eliminates the extra full-width status row and reduces empty header space.
- Responsive layout for smaller iPhones; app name truncates gracefully if customized long.
- No change to transaction data schema, storage keys, backup JSON structure or personalization.
- Retains AI Analyst, iPhone Export/Import, floating Add button, logo, icons, live date,
  service-worker offline caching and all original finance features.

INSTALLATION / UPDATE
1. Export a backup on EACH installed device, if possible, and verify it exists in Files.
2. Extract the ZIP. Upload ALL the app files (not the ZIP) to the SAME GitHub Pages
   publishing folder where that device originally installed the app.
3. Verify the live URL /version.json shows 1.7.5 (for a project site use
   https://USERNAME.github.io/REPOSITORY/version.json).
4. Open each existing app online, use Check for App Update, then fully reopen it.
5. Confirm footer shows v1.7.5 and the controls/date are aligned in the header.
6. After a successful online load, test offline launch.

CAUTION: DO NOT REMOVE EXISTING IPHONE HOME SCREEN INSTALLATIONS OR CLEAR WEBSITE
DATA. Financial transactions live on each phone. Changing a GitHub Pages URL
can leave existing installations unable to update. If friends installed from
/rico-finances/ and /personal-finances/, keep BOTH site addresses working.
First-time installation requires an internet connection.
No approved-device access-code security is implemented in this release.

Developer: Engr. Rico J. Pono

MY FINANCES v1.7.4 — LIVE HEADER DATE (CUMULATIVE OFFLINE EDITION)
================================================================

NEW IN v1.7.4
- Adds the current date directly beneath the personalized greeting.
- Example date: Monday, Nov. 2, 2026.
- Uses the phone's local date, updates periodically, and refreshes when the app is reopened or resumed.
- Preserves the header photo, app name, AI Analyst, floating Add button, settings,
  locally stored transaction data, offline functionality, and iPhone Export repair.
- App code version, visible footer, version.json, and service worker cache all updated to 1.7.4.

INSTALLATION
1. Export a backup first, if Export is available on the installed app.
2. Extract this ZIP and upload ALL app files (not the ZIP) to the existing GitHub Pages
   repository's publishing folder; keep the same Pages URL for existing users.
3. Check YOUR_GITHUB_PAGES_URL/version.json while online: it must show version 1.7.4.
4. Open the existing app online, use Check for App Update, and reopen it.
5. Verify the footer shows v1.7.4, the current date is beneath the greeting,
   and Export works before deleting any prior app or clearing browser data.
6. Open offline after an online launch has installed the updated files.

IMPORTANT
- All financial data is stored separately in each installation using the existing keys:
  rico_finances_txs and rico_finances_backup_fallback.
- Do NOT uninstall older Home Screen apps or clear website data until saved finance
  records have been exported and verified in Files.
- If /rico-finances/ and /personal-finances/ are both used by coworkers, publish
  app updates at the corresponding old and new URLs; renaming the repo alone is
  not a safe method of migrating local data.
- No private activation or approved-device restriction is included in this update.
- First-ever install requires internet; offline use requires one successful install.

Developed by: Engr. Rico J. Pono

RETAINED v1.7.3 REPAIR NOTES
----------------------------
MY FINANCES v1.7.3 — SAFE IPHONE EXPORT + UPDATE CHECK REPAIR
=========================================================

IMPORTANT: DO NOT DELETE THE OLD HOME SCREEN APP OR CLEAR SAFARI WEBSITE DATA.
Financial records are held locally in each app installation, not stored in GitHub.

REPAIRS
- Export now invokes native iPhone share sheet with a real .json File, when supported.
- If the share sheet is unavailable, Export opens a Backup Options dialog with
  Download and Copy backup text alternatives, plus a preview of the original JSON array.
- The backup timestamp changes only after user confirms a copy was saved.
- Update checker requests version.json BEFORE updating the service worker, and
  reports specific version-file/network failures rather than one generic error.
- Offline worker keeps version metadata checks truthful if there is no internet.
- Preserves all v1.7.2 finance features, original storage keys, AI Analyst,
  custom app name/greeting/photo, header, floating Add, and user-provided app logo.

TO INSTALL ON EXISTING GITHUB PAGES SITE
1. Upload all 13 actual app files (not this ZIP) to the SAME public Pages folder.
   You can replace repository app files; this does not delete data on users' phones.
2. Commit and wait for the site deployment to complete.
3. In Safari, visit YOUR_GITHUB_PAGES_URL/version.json (project page: /repo/version.json)
   and confirm that the JSON says version 1.7.3. HTTP 404 means the file isn't deployed
   at the address you're checking.
4. On the EXISTING installed app, stay online. Completely close it, then reopen it.
   Its earlier service worker uses network-first navigation, so it should get new HTML
   if the GitHub Pages deployment and connection are working.
5. Confirm the footer says v1.7.3, then tap Export and follow the iPhone share sheet
   or Backup Options to SAVE an actual personal copy of the transactions.
6. Verify the backup file exists in Files before removing or reinstalling anything.
7. Reopen offline AFTER at least one successful online load and cache install.

IF THE APP STILL SHOWS v1.7.1
- Check version.json at your live GitHub Pages URL in Safari.
- Check that Pages points to the branch/folder you updated (Settings > Pages).
- DO NOT delete your Home Screen app: existing offline and finance data may be lost.
- Try an online close/relaunch after confirming version.json on the website.

BACKUP FORMAT
JSON array identical to previous Export/Import, preserving compatibility.
Data keys remain rico_finances_txs and rico_finances_backup_fallback.
No financial transaction data is sent to the activation server or GitHub.

LIMITS
First installation needs internet. GitHub Pages is currently publicly accessible;
private one-time activation codes are NOT provided in this version.
Native iPhone share / Files UI depends on iOS and browser support.
The share sheet or download request is NOT proof of saved backup: verify in Files.

Developed by: Engr. Rico J. Pono
