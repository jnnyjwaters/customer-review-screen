# Customer Review Screen — public display mirror

This is a **public mirror**, not the source. It exists solely so
`index.html` can be served via GitHub Pages at a plain URL, no login, no
token, for systems that need a direct link rather than a downloadable
package.

- **Source of truth / actual build pipeline:** [jnnyjwaters/office-screens](https://github.com/jnnyjwaters/office-screens)
  (private — contains the review wall build script *and* the contacts/
  complaints wall, which stays private since it has real internal CS data).
- **This repo only ever contains `index.html`**, a synced copy of
  `screens/review-wall.html` from the private repo, refreshed every 30 min
  by `.github/workflows/sync_and_publish.yml`.
- Content here is intentionally public-safe: real App Store/Google Play
  reviews, which are already public on those platforms. Nothing internal
  (CS contact data, complaint drivers) is ever copied into this repo.

## Live URL

https://jnnyjwaters.github.io/customer-review-screen/

## If this breaks

Check the `SOURCE_REPO_TOKEN` secret hasn't expired (it's a read-only,
Contents-scoped token against `jnnyjwaters/office-screens`). Contact Jenny
Waters (jennyw@remitly.com).
