# sync-glitch-github-action

## Install

```
$ git clone git@github.com:glitch-tools/sync-glitch-github-action.git
$ cd sync-glitch-github-action
$ mv action-sync-glitch-github /path/to/your-repository/
```

## Usage

### Get required environment variables

1. Open your project on Glitch
1. Open devtool and click the Network tab
1. Select Project name > Advanced Options > Import from GitHub
1. You can find a request URL which starts from `https://api.glitch.com/projects/githubImport ~`:

   ![network](https://raw.githubusercontent.com/glitch-tools/sync-glitch-cli/master/public/assets/capture.png)

1. It has three params. These params are what you need.

### Create secrets variables on GitHub Action Editor

- `GLITCH_PROJECT_ID` _(the Glitch project id.)_
- `GLITCH_TOKEN` _(the Glitch authorization)_
