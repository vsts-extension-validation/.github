name: 'Add vsts extension to validate'
description: 'With this issue, you can add a GitHub hosted VSTS extension so we can validate it. When validating, we set-up codeQL analysis and run it against your extension. We also run a number of other checks to ensure your extension is ready for the marketplace.'
title: "[Add]: Please add <<organization>>/<<repo>> to the validation process"
body:
  - type: markdown
    attributes:
      value: |
        Thanks for taking the time to fill out this bug report!

  - type: input
    id: 'organization'
    attributes:
      label: 'Organization or user'
      description: 'Organization or user that owns the extension'
    validations:
      required: true

  - type: input
    id: 'repo'
    attributes:
      label: 'Which repository is the extension in?'
    validations:
      required: true
