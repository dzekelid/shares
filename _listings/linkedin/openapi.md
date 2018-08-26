---
swagger: "2.0"
x-collection-name: LinkedIn
x-complete: 1
info:
  title: LinkedIn
  description: bring-user-profiles-and-professional-networks-to-your-apps-
  version: 1.0.0
host: api.linkedin.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /people/shares:
    post:
      summary: Add People ~ Shares
      description: Post people ~ shares
      operationId: postPeople~Shares
      x-api-path-slug: peopleshares-post
      parameters:
      - in: header
        name: Content-Type
        description: The content type
      - in: query
        name: format
        description: The message format
        type: string
        format: string
      - in: header
        name: x-li-format
        description: The content type
      responses:
        200:
          description: OK
      tags:
      - People
      - Shares
  /companies/{id}/shares:
    post:
      summary: Add Companies Shares
      description: Post companies  shares
      operationId: postCompaniesShares
      x-api-path-slug: companiesidshares-post
      parameters:
      - in: query
        name: format
        description: The message format
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Companies
      - ""
      - Shares
---