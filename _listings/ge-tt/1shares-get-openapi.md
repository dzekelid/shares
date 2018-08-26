---
swagger: "2.0"
x-collection-name: Ge.tt
x-complete: 0
info:
  title: Ge.tt  REST API Shares
  description: 'Returns all your shares and the containing files:'
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