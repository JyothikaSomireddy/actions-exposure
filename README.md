# SecureStack GitHub Actions

A GitHub Action to execute SecureStack application attack surface analysis an application.

```
name: Example Workflow Using SecureStack Exposure Action
on: push
jobs:
  security:
    runs-on: ubuntu-latest
    steps:
      - name: Exposure Analysis Step
        id: exposure
        uses: SecureStackCo/actions-exposure@main
        with:
          securestack_api_key: ${{ secrets.SECURESTACK_API_KEY_SECRET }}
          securestack_app_id: ${{ secrets.SECURESTACK_APPI_ID }}
          severity: critical
          flags: '--dom'
```

## Getting your SecureStack API Key and Application ID

TODO

Made with 💜 by SecureStack
