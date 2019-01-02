# GitHub Action for Glitch

This Action for [Glitch](https://glitch.com/) enables arbitrary actions for interacting with Azure services via [the `sync-glitch` command line client.](https://github.com/glitch-tools/sync-glitch-cli)

## Usage

```hcl
# .github/main.workflow

workflow "Sync changes in your GitHub repository to glitch.com" {
  on = "push"
  resolves = ["Deploy"]
}

action "Deploy" {
  uses = "glitch-tools/sync-glitch-github-action@master"
  secrets = ["GLITCH_PROJECT_ID", "GLITCH_TOKEN"]
}
```

### Secrets

- `GLITCH_PROJECT_ID` - **Required** The `projectId` of yours.
- `GLITCH_TOKEN` – **Required** The `authorization` of yours.

For more details on [glitch-tools/sync-glitch-cli#how-to-get-required-environment-variables](https://github.com/glitch-tools/sync-glitch-cli#how-to-get-required-environment-variables)
