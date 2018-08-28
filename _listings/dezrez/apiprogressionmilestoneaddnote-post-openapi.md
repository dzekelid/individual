---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Add a note to an individual progression milestone
  version: 1.0.0
  description: Add a note to an individual progression milestone.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/accounting/exports/batch/{id}/removepayment:
    put:
      summary: Remove an individual payment from batch export
      description: Remove an individual payment from batch export.
      operationId: AccountingExport_RemoveFromBatchByidBypaymentId
      x-api-path-slug: apiaccountingexportsbatchidremovepayment-put
      parameters:
      - in: path
        name: id
      - in: query
        name: paymentId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Individual
      - Payment
      - From
      - Batch
      - Export
  /api/progression/milestone/addnote:
    post:
      summary: Add a note to an individual progression milestone
      description: Add a note to an individual progression milestone.
      operationId: Progression_AddMilestoneNoteBynoteDataContract
      x-api-path-slug: apiprogressionmilestoneaddnote-post
      parameters:
      - in: body
        name: noteDataContract
        description: Notes to be added
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Note
      - To
      - Individual
      - Progression
      - Milestone
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---