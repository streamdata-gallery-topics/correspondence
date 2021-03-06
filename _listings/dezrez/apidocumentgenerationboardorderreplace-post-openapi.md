---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Generates an board ordering Replace correspondence
  version: 1.0.0
  description: Generates an board ordering replace correspondence.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/documentgeneration/custompack:
    post:
      summary: Generates any correspondence and can allow you to overpost information
        to the correspondence
      description: Generates any correspondence and can allow you to overpost information
        to the correspondence.
      operationId: DocumentGeneration_GeneratePackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationcustompack-post
      parameters:
      - in: body
        name: generatePackDetails
        description: broad contract that allows for overposting and underposting,
          however you must specify a correspondence Id            you must then follow
          the validation rules for the for that individual correspondence type, each
          route to the controller is named in the same way            as the enumerated
          correspondence type system name, and the mappings for the specific class
          to the GeneratePackJobDataContract are detailed in             the each
          individual simplified contract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Any
      - Correspondence
      - Can
      - Ow
      - You
      - To
      - Overpost
      - Information
      - To
      - Correspondence
  /api/documentgeneration/boardordernew:
    post:
      summary: Generates an board ordering New correspondence
      description: Generates an board ordering new correspondence.
      operationId: DocumentGeneration_BoardOrderingNewPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationboardordernew-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Board
      - Ordering
      - New
      - Correspondence
  /api/documentgeneration/boardorderreplace:
    post:
      summary: Generates an board ordering Replace correspondence
      description: Generates an board ordering replace correspondence.
      operationId: DocumentGeneration_BoardOrderReplacePackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationboardorderreplace-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Board
      - Ordering
      - Replace
      - Correspondence
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