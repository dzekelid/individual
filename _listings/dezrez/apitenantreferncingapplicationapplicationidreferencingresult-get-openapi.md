---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Get the details of an individual application referencing result
  version: 1.0.0
  description: Get the details of an individual application referencing result.
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
  /api/progression/milestones/reset:
    put:
      summary: Add a note to an individual progression milestone
      description: Add a note to an individual progression milestone.
      operationId: Progression_ResetRoleMilestonesBypurchasingRoleIdByroleId
      x-api-path-slug: apiprogressionmilestonesreset-put
      parameters:
      - in: query
        name: purchasingRoleId
        description: The purchasing role ID
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: roleId
        description: Sales role ID
      responses:
        200:
          description: OK
      tags:
      - Note
      - To
      - Individual
      - Progression
      - Milestone
  /api/tenantreferncing/submitapplication/{caseId}:
    put:
      summary: Submits an individual referencing application for processing
      description: Submits an individual referencing application for processing.
      operationId: TenantReferencing_SubmitApplicationForReferencingBycaseId
      x-api-path-slug: apitenantreferncingsubmitapplicationcaseid-put
      parameters:
      - in: path
        name: caseId
        description: The id of the case to submit the application for
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Submits
      - Individual
      - Referencing
      - Applicationprocessing
  /api/tenantreferncing/application/{applicationId}/referencingresult:
    get:
      summary: Get the details of an individual application referencing result
      description: Get the details of an individual application referencing result.
      operationId: TenantReferencing_GetApplicationStatusByapplicationId
      x-api-path-slug: apitenantreferncingapplicationapplicationidreferencingresult-get
      parameters:
      - in: path
        name: applicationId
        description: The id of the application to retrieve results for
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Details
      - Of
      - Individual
      - Application
      - Referencing
      - Result
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