# War Diversity Planner

MCOC alliance war planner: member 7★ rosters, tap-to-assign defenders, duplicate checks, LINE-ready copy.
Saves to `data.json` in this repo, so every phone sees the same rosters and plan.

## Setup (about 10 minutes, one time)

1. **Create the repo.** On github.com tap **+ → New repository**. Name it `war-planner`, set it to **Public**, and tap **Create repository**.
2. **Upload the files.** On the new repo page tap **uploading an existing file**, drag in every file from this folder (`index.html`, `data.json`, `manifest.webmanifest`, the icons, this README), and tap **Commit changes**.
3. **Turn on the website.** Go to **Settings → Pages**. Under *Build and deployment* choose **Deploy from a branch**, branch **main**, folder **/ (root)**, then **Save**. After a minute the page shows your link, like `https://YOURNAME.github.io/war-planner/`.
4. **Make a save token (officers only).** Go to **Settings (your profile) → Developer settings → Personal access tokens → Fine-grained tokens → Generate new token**.
   - Expiration: up to 1 year
   - Repository access: **Only select repositories → war-planner**
   - Permissions → Repository permissions → **Contents: Read and write**
   - Generate, then copy the token (starts with `github_pat_`).
5. **Connect the app.** Open your link, go to **Alliance rosters → Save to GitHub → Officer setup**, paste the token, tap **Connect**. The owner and repo fill in automatically.

From then on every change saves to GitHub a few seconds after you stop tapping. The top-right status shows **Saved**.

## Using it

- **Members:** send them the link. They see the saved rosters and war plan (view only), and can build their own roster on **My roster** and send you the code in LINE. Add `#roster` to the link to open straight on My roster.
- **Home screen:** open the link in Safari/Chrome → Share → **Add to Home Screen**. It opens like an app.
- **Other officers:** each makes their own token (step 4, from an account with write access to the repo) and connects on their own phone.
- **History:** every save is a commit, so you can see or restore any older version under the repo's **History** for `data.json`.

## Notes

- Keep the token private. It only works on this one repo, and you can revoke it anytime under Developer settings.
- The GitHub Pages copy of `data.json` can lag about a minute behind; the app reads GitHub directly, so it's normally current.
- Screenshot reading isn't in this version; it needs Claude. Send screenshots to Claude for roster codes instead.
