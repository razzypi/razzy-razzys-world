# Repository Synchronization

This repository automatically syncs to the HowWeBuilt organization with the naming convention `howwebuilt/razzy-razzys-world`.

## How It Works

1. Changes pushed to this repository (razzypi/razzy-razzys-world) trigger a GitHub Action
2. The action pushes the same changes to `howwebuilt/razzy-razzys-world`
3. This allows the Vercel deployment to access the repository under the howwebuilt account

## Requirements

- `RAZZY_GITHUB_TOKEN`: Personal access token for the razzy account (read access)
- `HOWWEBUILT_GITHUB_TOKEN`: Personal access token for the howwebuilt account (write access to destination repo)

## Branch Mapping

- All branches and tags are synchronized from razzy/razzy-razzys-world to howwebuilt/razzy-razzys-world

## Manual Sync

You can manually trigger the sync using the "workflow_dispatch" option in the GitHub Actions tab.