# GitHub Dashboard

A published web application for exploring and sharing GitHub profile stats.

The dashboard lets you check activity, streaks, languages, top repositories, and recent commits, then share results as text or an image.

![GitHub Dashboard Screenshot](.github/torvalds-github.png)

## Live App

- Website: https://pseudozoid.github.io/gitdash/

## Features

- Load any public GitHub username
- View yearly contributions and activity heatmap
- See current and longest streaks
- Review recent commits
- Check top languages and top repositories
- Track simple personal goals
- Share stats by:
  - copying text
  - downloading a text summary
  - downloading a screencap

## How To Use

1. Open the live app at https://pseudozoid.github.io/gitdash/
2. Enter a GitHub username
3. Click **Load**

Optional: add a GitHub token for more reliable and accurate results.

## GitHub Token (Optional, Recommended)

Using a personal access token provides:

- **Better reliability**: authenticated requests have higher rate limits
- **Fewer API limit issues**: 60 requests/hour without token vs. 5,000 with token
- **Accurate contributions**: GitHub's public API sometimes undercounts contributions; tokens access the private contribution calendar API for exact counts

### How to Get a Token

1. Open [GitHub Personal Access Tokens page](https://github.com/settings/tokens/new)
2. Set token details:
   - Token name: `gitdash` (or your chosen name)
   - Expiration: 90 days (or your preference)
   - Select scopes: check **`public_repo`** (read-only access to public repos)
3. Click "Generate token" at the bottom
4. Copy the token (shown only once)
5. Paste into the "GitHub token" field in the dashboard and click **Load**

### Token Security

- The token is **stored only in your browser's local storage**—never sent to any server except GitHub
- Tokens are **masked when exporting screencaps** (shows `****` instead of the actual token)
- You can revoke the token anytime in [GitHub settings](https://github.com/settings/tokens)
- This app is open-source; you can inspect the code to verify no tokens are logged or transmitted elsewhere

## Sharing Stats

Use the share buttons at the top of the dashboard:

- **Copy stats text**
- **Download stats text**
- **Download screencap**

## Troubleshooting

- Add a token if totals seem too low.
- Reload if GitHub rate limits are hit.
- Some profiles may show limited commit info if recent public activity is low.

## Project Structure

- `index.html` - production entrypoint for the published app

## Roadmap & Future Improvements

Planned enhancements to reduce friction and add features:

- **GitHub OAuth Login** — seamless login via GitHub without manual token entry; token handled securely server-side
- **Contribution Streak Tracking** — persist and visualize your streaks over time
- **Dark/Light Theme Toggle** — theme preference storage
- **Comparison Mode** — side-by-side stats for multiple GitHub users
- **Advanced Sharing** — embed dashboard widget in blogs/portfolios
- **Auto-Refresh** — optional periodic updates to stats without manual reload

Contributions and suggestions welcome!
