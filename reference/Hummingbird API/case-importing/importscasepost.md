---
title: Import cases
excerpt: >-
  This endpoint will allow you to import multiple cases at once. The POST body
  should conform to the newline-delimited <a
  href="https://jsonlines.org/">JSONLines</a> format. Each case should resemble
  a <a
  href="https://docs.hummingbird.co/#tocS_CaseCreateRequest">CaseCreateRequest</a>
  object, and each case should take up exactly one line, with a newline
  separating out the cases. The cases are all imported as a background job. This
  endpoint will return to you a token that you can use to lookup the status of
  the cases.
api:
  file: oas.json
  operationId: imports_case_post
hidden: false
---