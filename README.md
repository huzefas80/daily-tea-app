# Daily Tea App

Public code-only frontend for Daily Pour. No beverage records or access tokens are included in this repository.

## Enable hosting

Open Settings → Pages. Under Build and deployment, choose Deploy from a branch, main, /(root), and Save. GitHub displays the live site URL after deployment.

## Connect your private records

Open the live app. The GitHub owner and private data repository are prefilled. Enter an expiring fine-grained personal access token restricted to the private data repository with Contents: read and write. Enter the token only inside the app, never in a repository file or chat. The ChatGPT GitHub connection does not automatically authenticate the standalone web page.

Click Connect & load. Entries are loaded from the private repository's data/entries.json. Changing a drink saves to that private file. Wait for Saved to GitHub. The token is held only in memory and must be reentered after a page refresh. You may also download index.html and use it locally while saving records remotely.

## Privacy

Keep the data repository private and never copy its data directory here. This app is public; its records are fetched only through authenticated GitHub API requests. Do not add third-party scripts or analytics that could inspect runtime credentials. Sundays are excluded from displayed tables, totals and CSV exports. Backups retain imported records.

## Verification status

Code and simulated sync checks passed. Live user-token sign-in and browser saving need a one-time verification after hosting is enabled. Google Sheets is not automatically synced.
