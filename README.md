# Nova Launcher wallpapers

`wallpapers.json` is the catalog, `images/` holds the WebP files.
Publish this folder as a public GitHub repo, then in Firebase Remote Config set `wallpaper_manage`:

    {"wallpaper_status":"on","wallpaper_base_url":"https://cdn.jsdelivr.net/gh/teamblackatom-create/nova-wallpapers@main/"}

To add a wallpaper: put the .webp in `images/` and add a row to `wallpapers.json`
({"id","name","category","file","pro","price"}). Categories: Gradient, Nature, Space, 3D, Artistic, Dark, Krishna, Aesthetic.
jsDelivr caches for a while; use a tag or commit hash in the URL (`@v2`) when you need a change to show at once.

## themes/ folder
`themes/` holds the full theme pictures (`st_pv_*` previews and `st_wp_*` wallpapers). The app keeps only a tiny blurred copy of each and
downloads the full picture from `<base>/themes/<name>.webp` the first time it is shown. Keep file names exactly as they are.
