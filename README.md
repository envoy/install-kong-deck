# Install Kong Gateway Deck
Github Action to install Kong Gateway CLI Deck. The Github action can enable CI to deploy the kong declarative configuration (yml files) to sync with the Kong Gateway using `deck` CLI.

## Inputs

Name | Description | Required
--- | --- | ---
`version` | Deck CLI version to install | `true`

## Example Usage

```
jobs:
  install-deck:
    runs-on: ubuntu-latest
    steps:
    - name: Install Kong Deck CLI
        uses: envoy/install-kong-deck@v1.0.0
        with:
          # Kong Deck CLI Version to install (Mandatory)
          version: 1.0.0
```

## Local Development

Refer [this](https://docs.github.com/en/actions/creating-actions/creating-a-composite-action) document to learn more on how to create custom Github Actions (composite) 
