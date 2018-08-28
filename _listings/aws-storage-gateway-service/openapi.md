swagger: "2.0"
x-collection-name: AWS Storage Gateway Service
x-complete: 1
info:
  title: AWS Storage Gateway Service API
  version: 1.0.0
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