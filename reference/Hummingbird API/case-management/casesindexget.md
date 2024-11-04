---
title: List cases
excerpt: >-
  List existing cases, filtered as specified by query parameters.

  This endpoint follows Relay conventions for pagination. Cursors are only
  applicable to the current query and cannot be re-used with different filter
  parameters.

  Only cases from the organization associated with the credentials provided in
  the Authorization header will be returned.

  Unless otherwise noted, results are returned in ascending order by their
  createdAt timestamp.

  Example request: `GET /cases?createdBetween=2020-08-01...2021-09-02`
api:
  file: oas.json
  operationId: cases_index_get
hidden: false
---