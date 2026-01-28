TusarTheme  RStudio editor theme

A dark, polished editor theme for RStudio (formerly packaged as Yule-based). This repository contains `TusarTheme.rstheme` and preview images.

![](images/mockup-rstudio.png)

Highlights
- Candy-cane style line highlight (subtle)
- Optional cursor animation
- Tuned for RStudio / Posit dark UI

Installation

Run this in R (RStudio recommended):

```r
theme_file <- fs::path_temp("TusarTheme", ext = "rstheme")
download.file(
  "https://raw.githubusercontent.com/imtrt004/TusarTheme/main/TusarTheme.rstheme",
  theme_file,
  mode = "wb"
)
rstudioapi::addTheme(theme_file, apply = TRUE)
```

Manual installation

1. Download `TusarTheme.rstheme` from this repository.
2. Copy it to the `~/.R/rstudio/themes` directory (or the path returned by `fs::path_home_r(".R", "rstudio", "themes")`).
3. In RStudio Preferences  Appearance, choose `TusarTheme`.

Disable cursor animations

If you prefer to disable cursor animations, edit the installed theme file (`~/.R/rstudio/themes/TusarTheme.rstheme`) and remove or comment out `animation-*` CSS rules under `.ace_cursor` and `.normal-mode .ace_cursor`.

Notes
- Best experienced with the RStudio dark UI.
- Restart RStudio if the theme doesn't show immediately after installation.

Contributing

Contributions, bug reports, and suggestions are welcome. Please open an issue or submit a pull request: https://github.com/imtrt004/TusarTheme

Credits

- Theme adapted for RStudio by the repository owner.

License

See the `LICENSE` file for license details.

Preview images are in the `images/` folder.

Enjoy!
