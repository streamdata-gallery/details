---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Blockchain Data Integrity Post Proxy Signature Details
  description: Post proxy signature details.
  contact:
    name: Ericsson - dcs.support@ericsson.com
  version: 1.0.0
host: bcdi-proxy-service.run.aws-usw02-pr.ice.predix.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/proxy/signature/details:
    post:
      summary: Post Proxy Signature Details
      description: Post proxy signature details.
      operationId: postV1ProxySignatureDetails
      x-api-path-slug: v1proxysignaturedetails-post
      parameters:
      - in: header
        name: Authorization
        description: token
      - in: header
        name: Predix-Zone-Id
        description: serviceInstanceId
      - in: body
        name: request
        description: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Proxy
      - Signature
      - Details
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