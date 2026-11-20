# Tero Games website

Plain HTML/CSS, no build step. Push it to GitHub and turn on **Settings → Pages → Deploy from branch (main, / root)**.

```
index.html                         Tero Games home (all games)
tero/index.html                    Tero
tero/privacy/                      Tero privacy policy
tero/support/                      Tero support page (the App Store "Support URL")
terrifico/index.html               Terrifico
terrifico/privacy/                 Terrifico privacy policy
terrifico/support/                 Terrifico support page (the App Store "Support URL")
rico-safari-salon/index.html       Rico's Safari Salon
rico-safari-salon/privacy/         Rico's Safari Salon privacy policy
app-ads.txt                        AdMob seller file
```

## Adding store links

Each game page has two buttons (Google Play, App Store) marked with an HTML comment:

```html
<!-- Paste the Google Play URL in href (replace "#") -->
<a class="store" href="#" data-store="google-play" ...>
```

While `href="#"` the button is dimmed with a "Coming soon" badge. Put the real URL in `href` and it turns
into a normal working button. No other change is needed. To drop a store, delete its `<a class="store">` block.

## Privacy policy URLs (for Play Console)

Replace `USER.github.io/REPO` with your Pages address:

- `https://USER.github.io/REPO/tero/privacy/`
- `https://USER.github.io/REPO/terrifico/privacy/`
- `https://USER.github.io/REPO/rico-safari-salon/privacy/`

The policies are copies of the ones in each game folder. If you edit a policy, update both copies.
