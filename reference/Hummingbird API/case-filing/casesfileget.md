---
title: Validate a case before filing
excerpt: >-
  This endpoint will run validations against the case with the given token, but
  will not file. This can be used as a pre-filing test endpoint to verify that
  your filing has no known validation errors for the jurisdiction specified.
  Returns any validation errors if there are any. Returns an error if the case
  does not exist. Returns a success status if all validations are run without
  error.
api:
  file: oas.json
  operationId: cases_file_get
hidden: false
---