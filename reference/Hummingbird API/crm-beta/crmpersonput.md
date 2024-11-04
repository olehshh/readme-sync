---
title: Add or update a person
excerpt: >-
  Create a new person or multiple people. If a person with the same ID exists,
  it will update fields of the existing record instead. If any errors are
  encountered during creation the endpoint will return an object with one or
  more descriptive errors. The request to this endpoint is expected to have one
  or more named fields associated with the person; any field omitted from the
  request will be left in its current state. Declaring a field in the request
  body, even if the field is explicitly set to null, will result in the field
  being updated.

  If create/update are successful, the response body will contain an object with
  all fields for the person. If any failures occur the response body will
  provide an error message with details.
api:
  file: oas.json
  operationId: crm_person_put
hidden: false
---