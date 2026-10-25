# Profile README — maintenance notes

This is the profile repository for **[@prashantrix](https://github.com/prashantrix)**. The README follows a visual portfolio layout: animated analyst hero, analytics approach, toolkit, ID/dashboard panel, featured projects, contribution landscape, and contact panel.

## Files displayed on the profile

- `README.md` — layout and featured analytics projects.
- `assets/hero.svg` — animated terminal, cycling roles, open-to-work pill, and the anime intro clip (72 embedded frames from a camera-stabilised video, shown in a viewfinder frame).
- `assets/off-the-clock.svg` — anime and gym carousel with story-style progress bars.
- `assets/about-life.svg` — an analytics workflow and working principles.
- `assets/stack.svg` — SQL, PostgreSQL, Excel, Python, and Power BI.
- `assets/id-dashboard.svg` — analyst ID and dashboard concept.
- `assets/connect.svg` — contact call-to-action.
- `assets/anime-data-analyst.png` — original artwork (no longer used inside the SVGs; kept as a source file).
- `profile-3d-contrib/profile-night-view.svg` — generated contribution landscape.

## Workflows

- `.github/workflows/profile-3d.yml` generates the 3D contribution visuals.
- `.github/workflows/github-snake.yml` generates contribution-snake files on its schedule. The current README prioritizes the portfolio layout and does not display the snake section.

## Updating the profile

1. Update the project table in `README.md` when a project or tool changes.
2. Keep image paths relative to the repository root.
3. When changing an SVG, increment its `?v=` query parameter in `README.md` to help GitHub refresh cached images.
4. Check the repository's **Actions** tab if the contribution landscape is stale or a workflow fails.

The extra `lanyard.svg`, `stats.svg`, `langs.svg`, and `trophies.svg` files are optional design elements retained from the profile guide; they are not part of the current compact layout.
