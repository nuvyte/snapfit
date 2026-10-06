# snapfit-site

Published as a GitHub Pages site at:
`https://nuvyte.github.io/snapfit/`

It hosts the Snapfit landing page, the privacy policy, and `version.json`, which the app reads on launch.

## Forcing or suggesting an update
```json
{ "minVersionCode": 2, "latestVersionCode": 2, "message": "A new version of Snapfit is ready." }
```
- `minVersionCode`: anyone below this sees a full-screen "Update needed" card they can't dismiss.
- `latestVersionCode`: anyone below this (but at or above min) gets a tappable toast, at most once a day.
- `message`: text on the "Update needed" card.

Commit and push; it's live within a few minutes. Players who are offline are never blocked.

- Privacy policy URL for Play Console: `https://nuvyte.github.io/snapfit/privacy-policy.html`
- The source copy of the policy lives in `../store/privacy-policy.html`; keep the two in sync.

## Publishing with GitHub Pages
1. Push this repo to `github.com/nuvyte/snapfit`.
2. In the repo, go to **Settings → Pages**.
3. Under **Source**, choose **Deploy from a branch**, branch `main`, folder `/ (root)`.
4. Click **Save**; the site goes live in a minute or two.
