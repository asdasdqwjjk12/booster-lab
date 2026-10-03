Booster Lab — online Google Sites + jsDelivr export

IMPORTANT — publish the updated Booster Lab app to Replit BEFORE uploading these
CDN files or replacing the Google Sites embed code. The deployed production
backend must include the anonymous guest-trading routes. The existing public
app URL alone is not enough: an older deployment can still load at that URL
while its backend lacks those routes. Wait for the updated Replit deployment to
complete before continuing; otherwise embedded trading will not work.

The CDN hosts only the Booster Lab frontend and static game images. Anonymous
online trading requires the updated live backend at https://fair-trade-forge.replit.app. This embed is
for anonymous guest trading only. Live account sign-in and account-specific
features are separate: the Google Sites code does not embed Clerk or a live
account session. Use the live Booster Lab app for account-based features.
All money, grading and rewards are simulated gameplay, not real transactions.

The Google Sites document is configured for anonymous online use. It initializes
BOOSTER_EMBEDDED_GUEST=true, BOOSTER_OFFLINE=false, BOOSTER_API_BASE=https://fair-trade-forge.replit.app,
and BOOSTER_ASSET_BASE=https://cdn.jsdelivr.net/gh/asdasdqwjjk12/booster-lab@main/

Update an existing public repo (small ZIP):
1. First publish the updated Replit app and wait for the deployment to complete,
   as described above. Do not upload the new CDN files or replace the embed
   before the guest-trading backend routes are live.
2. Extract booster-lab-jsdelivr-online.zip and upload its new versioned .js and .css files
   to the ROOT of https://github.com/asdasdqwjjk12/booster-lab. Upload
   google-sites-embed.html and embed-code.txt for your records.
3. Keep older versioned JS/CSS files: an already-published embed may still use
   one of those immutable URLs. Do not rename the new files to booster-lab.js/css.
4. Paste all of embed-code.txt in Google Sites: Insert > Embed > Embed code.
   The document includes a viewport meta tag and a small iframe-safe reset.
   Set the Sites embed tall enough for the app and publish.
5. Open the newly published page and test embedded anonymous trading. The
   backend must allow requests from the published site's origin.

For a mounted QA preview, place local-preview.html and its hashed JS/CSS files
beside one another at /cdn-check/. It uses this repo's CDN as its image base, so
the two large image folders do not need to be copied to the web app.

The small update ZIP intentionally omits pack-images and crown-card-images,
which are already present in your public repo. For a first-time upload or to
refresh every image, use booster-lab-jsdelivr-online-full.zip and upload both
image folders at the repository root, preserving their names and paths.
