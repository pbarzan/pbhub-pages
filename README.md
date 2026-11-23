# pbhub-pages

Static pages required by the Enable Banking application registration for **PB Hub**,
a personal, single-user Android app. Published with GitHub Pages.

| File | Purpose |
|---|---|
| `index.html` | Landing page |
| `privacy.html` | Privacy policy (required by Enable Banking) |
| `terms.html` | Terms of use (required by Enable Banking) |
| `callback.html` | OAuth redirect bridge: forwards `code`/`state` to the `pbhub://` custom scheme |

`callback.html` runs entirely client-side. It never transmits the authorization code
anywhere: it only rewrites the current URL to the app's custom scheme and offers it for
manual copy as a fallback.

No build step, no dependencies, no analytics.
