# Nova Launcher wallpapers

`wallpapers.json` is the catalog, `images/` holds the WebP files.
Publish this folder as a public GitHub repo, then in Firebase Remote Config set `wallpaper_manage`:

    {"wallpaper_status":"on","wallpaper_base_url":"https://cdn.jsdelivr.net/gh/<user>/<repo>@main/"}

To add a wallpaper: put the .webp in `images/` and add a row to `wallpapers.json`
({"id","name","category","file","pro","price"}). Categories: Gradient, Nature, Space, 3D, Artistic, Dark, Krishna, Aesthetic.
jsDelivr caches for a while; use a tag or commit hash in the URL (`@v2`) when you need a change to show at once.
