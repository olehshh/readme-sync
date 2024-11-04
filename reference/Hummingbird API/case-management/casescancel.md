---
title: Cancel a case
excerpt: >-
  Cancel an existing case with the given token and all of the reviews within it.
  This operation requires that the case and all its reviews be eligible for
  cancellation, i.e. the case is neither locked nor merging, and none of its
  reviews have been filed. Returns an error if the case does not exist or if it
  cannot be cancelled. Returns a success status if the case was successfully
  cancelled.
api:
  file: oas.json
  operationId: cases_cancel
hidden: false
---