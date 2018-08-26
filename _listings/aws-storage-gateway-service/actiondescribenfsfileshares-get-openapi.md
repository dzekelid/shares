---
swagger: "2.0"
x-collection-name: AWS Storage Gateway Service
x-complete: 0
info:
  title: AWS Storage Gateway Service API Describe NFS File Shares
  version: 1.0.0
  description: Gets a description for one or more file shares from a file gateway.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeNFSFileShares:
    get:
      summary: Describe NFS File Shares
      description: Gets a description for one or more file shares from a file gateway.
      operationId: describeNFSFileShares
      x-api-path-slug: actiondescribenfsfileshares-get
      parameters:
      - in: query
        name: FileShareARNList
        description: An array containing the Amazon Resource Name (ARN) of each file
          share to be described
        type: string
      responses:
        200:
          description: OK
      tags:
      - NFS File Shares
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