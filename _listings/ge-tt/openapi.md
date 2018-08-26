---
swagger: "2.0"
x-collection-name: Ge.tt
x-complete: 1
info:
  title: Ge.tt  REST API
  description: the-ge-tt-api-allows-you-to-use-ge-tt-in-your-own-applications--we-believe-that-our-users-should-be-able-to-access-their-files-and-share-their-content-in-their-platform-of-choice--by-using-the-api-developers-are-able-to-easily-put-their-own-content-or-the-content-of-their-users-online--at-the-same-time-they-are-able-to-use-ge-tts-unique-realtime-file-sharing-technology-where-files-are-available-before-they-are-even-uploaded-
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
---