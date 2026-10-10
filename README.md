# Pastel

A soft, professional Redmine theme that is easy on the eye: pastel blue-grey
surfaces with deep ocean blue structure and deep teal, emerald and
deep maroon accents.

## Installation

1. Clone this theme ([https://github.com/zaburt/redmine_pastel](https://github.com/zaburt/redmine_pastel)) into the Redmine `themes/`
   directory at the application root (Redmine 7+) as `pastel`:

   ```
   git clone https://github.com/zaburt/redmine_pastel.git themes/pastel
   ```

   The result should contain:

   ```
   themes/pastel/stylesheets/application.css
   ```

   > Note: Redmine 6 and earlier used `public/themes/` instead of `themes/`.

2. Restart Redmine. In production, precompile assets:

   ```
   RAILS_ENV=production bin/rails assets:precompile
   ```

3. Go to `Administration -> Settings -> Display` and select "Pastel"
   in the "Theme" drop-down list.

## Customize

1. Change `images/logo.svg` for the header logo, `images/logo-login.svg` for
   the login page and `favicon/favicon.svg` for the browser tab icon.
2. The palette is defined inline as hex values in
   `stylesheets/application.css`:

   | Role                     | Color     |
   |--------------------------|-----------|
   | Ocean cerulean (base)    | `#00557F` |
   | Deep teal                | `#007F7F` |
   | Deep emerald (success)   | `#007F55` |
   | Rose (hover accent)      | `#A8465F` |
   | Dark wine (alerts)       | `#5E0020` |
   | Deep maroon (accent)     | `#7F002A` |

   Surfaces and text are tints of blue-grey derived from the base hue.
3. In production, re-run `assets:precompile` after editing any theme file.

## License

Licensed under [GNU GPLv2](LICENSE).

Copyright (c) 2026 Onur Küçük (onur [at] delipenguen.net)
