---
name: RTI
about: Track an RTI application
title: TC
labels: ''
assignees: ''

---

name: New RTI Application
description: File a new Right to Information request
title: "RTI: [Brief Subject]"
labels: ["02 Filed"]
body:
  - type: markdown
    attributes:
      value: |
        ## RTI Application Details
  - type: input
    id: rti_reg_no
    attributes:
      label: RTI Registration No.
      placeholder: e.g., RTI/2023/12345
    validations:
      required: false
  - type: input
    id: pio_name
    attributes:
      label: PIO Name
      placeholder: e.g., Mr. Suresh Kumar
  - type: dropdown
    id: district
    attributes:
      label: District
      options:
        - Kerala
        - Thrissur
        - Palakkad
        - Trivandrum
        - Other
    validations:
      required: true
  - type: input
    id: department
    attributes:
      label: Department
      placeholder: e.g., Water Authority, Education
  - type: textarea
    id: description
    attributes:
      label: Information Requested
      description: Briefly describe what information was sought.
    validations:
      required: true
  - type: input
    id: expense
    attributes:
      label: Total Expense (₹)
      placeholder: e.g., 10
