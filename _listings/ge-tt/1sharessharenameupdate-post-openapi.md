---
swagger: "2.0"
x-collection-name: Ge.tt
x-complete: 0
info:
  title: Ge.tt  REST API Shares Update
  description: Updates a share. Currently you can only update the title
  termsOfService: http://ge.tt/terms
  version: "1"
host: open.ge.tt
basePath: /1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /1/shares:
    get:
      summary: Shares
      description: 'Returns all your shares and the containing files:'
      operationId: get1Shares
      x-api-path-slug: 1shares-get
      parameters:
      - in: query
        name: accesstoken
      responses:
        200:
          description: OK
      tags:
      - Shares
  /1/shares/create:
    post:
      summary: Shares Create
      description: 'Creates a new share. The request body is optional but can look
        like:'
      operationId: post1SharesCreate
      x-api-path-slug: 1sharescreate-post
      parameters:
      - in: query
        name: accesstoken
      responses:
        200:
          description: OK
      tags:
      - Shares
      - Create
  /1/shares/{sharename}:
    get:
      summary: Shares
      description: Lists a share.
      operationId: get1SharesSharename
      x-api-path-slug: 1sharessharename-get
      parameters:
      - in: path
        name: sharename
      responses:
        200:
          description: OK
      tags:
      - Shares
      - Sharename
  /1/shares/{sharename}/destroy:
    post:
      summary: Shares Destroy
      description: Delete a share and all of its files.
      operationId: post1SharesSharenameDestroy
      x-api-path-slug: 1sharessharenamedestroy-post
      parameters:
      - in: query
        name: accesstoken
      - in: path
        name: sharename
      responses:
        200:
          description: OK
      tags:
      - Shares
      - Sharename
      - Destroy
  /1/shares/{sharename}/update:
    post:
      summary: Shares Update
      description: Updates a share. Currently you can only update the title
      operationId: post1SharesSharenameUpdate
      x-api-path-slug: 1sharessharenameupdate-post
      parameters:
      - in: query
        name: accesstoken
      - in: path
        name: sharename
      responses:
        200:
          description: OK
      tags:
      - Shares
      - Sharename
      - Update
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