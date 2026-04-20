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

Using a token helps with:

- better reliability
- fewer API limit issues
- more accurate contribution totals

The token is stored in your browser for convenience and is masked when exporting screencaps.

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
