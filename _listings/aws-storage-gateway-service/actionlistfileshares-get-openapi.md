---
swagger: "2.0"
x-collection-name: AWS Storage Gateway Service
x-complete: 0
info:
  title: AWS Storage Gateway Service API List File Shares
  version: 1.0.0
  description: Gets a list of the file shares for a specific file gateway, or the
    list of file shares that belong to the calling user account.
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
  /?Action=ListFileShares:
    get:
      summary: List File Shares
      description: Gets a list of the file shares for a specific file gateway, or
        the list of file shares that belong to the calling user account.
      operationId: listFileShares
      x-api-path-slug: actionlistfileshares-get
      parameters:
      - in: query
        name: GatewayARN
        description: The Amazon resource Name (ARN) of the gateway whose file shares
          you want to list
        type: string
      - in: query
        name: Limit
        description: The maximum number of file shares to return in the response
        type: string
      - in: query
        name: Marker
        description: Opaque pagination token returned from a previous ListFileShares
          operation
        type: string
      responses:
        200:
          description: OK
      tags:
      - File Shares
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