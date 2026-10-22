# Setup — prashantrix animated GitHub profile

## Files
- `README.md` — profile content (put in the root of `prashantrix/prashantrix`)
- `assets/banner.svg` and `assets/banner-light.svg` — animated neon banner with embedded anime artwork
- `assets/anime-data-analyst.png` — standalone original character art
- `assets/lanyard.svg` — swinging ID badge animation
- `assets/stats.svg`, `assets/langs.svg`, `assets/trophies.svg` — local decorative cards
- `.github/workflows/github-snake.yml` — daily contribution snake workflow

## Install
1. Open https://github.com/prashantrix/prashantrix. If this repository does not exist, create a **public** repository named exactly `prashantrix` (the username) and initialize it with a README.
2. Download and unzip this package.
3. Upload the contents of this folder to the repository root, preserving the `assets/` and `.github/workflows/` folders. Do not upload the outer zip or outer parent folder itself.
4. Commit the changes to the default branch (usually `main`).
5. Open the repository's **Settings → Actions → General**. Under Workflow permissions, choose **Read and write permissions** if your organization/account policy allows it. Save.
6. Open **Actions**, enable workflows if prompted, select **Generate contribution snake**, and choose **Run workflow**. Wait for the run to complete.
7. Check that an `output` branch was created and that it contains the snake SVGs. If your account policy prevents write access, the action will fail; fix the repository Actions permission or use a forked/alternative publishing method.
8. Check the profile at https://github.com/prashantrix and test both light and dark GitHub themes.

## Before you publish
- The Seasonal Agriculture Performance Analysis link has been verified: https://github.com/prashantrix/Seasonal-Agriculture-Performance-Analysis.
- The public email is included because you explicitly supplied it. Remove it if you do not want it exposed.
- Replace the LinkedIn/social placeholder with your actual public profile links if desired.
- External GitHub Stats cards can be rate-limited; the local SVG cards are decorative fallback cards, not live metrics.
- SVG SMIL/CSS animations usually work in GitHub-rendered SVG images, but GitHub sanitizes SVG content. Embedded image and animation behavior can vary by renderer; test the final commit. If a banner is blocked, use the PNG artwork as a static fallback.
- The generated character art is stylized, not a photorealistic likeness.
- GitHub strips JavaScript from README content; this package uses SVG/CSS animation only.
- If you edit a local image and GitHub shows a cached version, increment the `?v=1` query string in README.

## Security
The workflow requests `contents: write` only to publish the generated files to the `output` branch. It uses the repository's built-in `GITHUB_TOKEN`; no personal access token is required. Never put a personal access token or password in the README or workflow.
