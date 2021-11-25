# `deploy-docker` - **Github Action**

This action deploy docker image

## Input

| Name               | Description                                                                                    |
| ------------------ | ---------------------------------------------------------------------------------------------- |
| `registry-username`| Username for image registry                                                                    |
| `registry-password`| Password for image registry                                                                    |

## Example Workflow File

```yaml
name: Build maven project and deploy docker image

on: [pull_request]

jobs:
  deploy:
    runs-on: ubuntu-latest
      steps:
        uses: rbkmoney/build-actions/packages/deploy-docker@v1.0.0
```