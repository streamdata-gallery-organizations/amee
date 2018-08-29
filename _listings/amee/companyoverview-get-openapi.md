---
swagger: "2.0"
x-collection-name: AMEE
x-complete: 0
info:
  title: AMEE Company API Get Company Overview
  description: Get company overview.
  version: "1.0"
host: api.roaring.io
basePath: /company/1.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /company-board-members:
    get:
      summary: Get Company Board Members
      description: Get company board members.
      operationId: getCompanyBoardMembers
      x-api-path-slug: companyboardmembers-get
      parameters:
      - in: query
        name: companyId
        description: Company identification for the company
      - in: query
        name: countryCode
        description: Country code for the company
      responses:
        200:
          description: OK
      tags:
      - Company
      - Board
      - Members
    post:
      summary: Post Company Board Members
      description: Post company board members.
      operationId: postCompanyBoardMembers
      x-api-path-slug: companyboardmembers-post
      parameters:
      - in: body
        name: body
        description: Request body with company identifiers to lookup
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: countryCode
        description: Country code for the company
      responses:
        200:
          description: OK
      tags:
      - Company
      - Board
      - Members
  /company-credit-decision:
    get:
      summary: Get Company Credit Decision
      description: Get company credit decision.
      operationId: getCompanyCreditDecision
      x-api-path-slug: companycreditdecision-get
      parameters:
      - in: query
        name: companyId
        description: Company identification for the company
      - in: query
        name: countryCode
        description: Country code for the company
      - in: query
        name: template
        description: Template for credit decision
      responses:
        200:
          description: OK
      tags:
      - Company
      - Credit
      - Decision
  /company-economy-overview:
    get:
      summary: Get Company Economy Overview
      description: Get company economy overview.
      operationId: getCompanyEconomyOverview
      x-api-path-slug: companyeconomyoverview-get
      parameters:
      - in: query
        name: companyId
        description: Company identification for the company
      - in: query
        name: countryCode
        description: Country code for the company
      responses:
        200:
          description: OK
      tags:
      - Company
      - Economy
      - Overview
    post:
      summary: Post Company Economy Overview
      description: Post company economy overview.
      operationId: postCompanyEconomyOverview
      x-api-path-slug: companyeconomyoverview-post
      parameters:
      - in: body
        name: body
        description: Request body with company identifiers to lookup
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: countryCode
        description: Country code for the company
      responses:
        200:
          description: OK
      tags:
      - Company
      - Economy
      - Overview
  /company-event:
    post:
      summary: Post Company Event
      description: Post company event.
      operationId: postCompanyEvent
      x-api-path-slug: companyevent-post
      parameters:
      - in: body
        name: body
        description: Request body with company identifiers to lookup
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: countryCode
        description: Country code for the company
      responses:
        200:
          description: OK
      tags:
      - Company
      - Event
  /company-overview:
    get:
      summary: Get Company Overview
      description: Get company overview.
      operationId: getCompanyOverview
      x-api-path-slug: companyoverview-get
      parameters:
      - in: query
        name: companyId
        description: Company identification for the company
      - in: query
        name: countryCode
        description: Country code for the company
      responses:
        200:
          description: OK
      tags:
      - Company
      - Overview
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