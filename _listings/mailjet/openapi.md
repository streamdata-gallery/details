swagger: "2.0"
x-collection-name: Mailjet
x-complete: 1
info:
  title: Mailjet Messages API
  description: allows-you-to-list-and-view-the-details-of-a-message-an-email-processed-by-mailjet
  version: v3
host: api.mailjet.com
basePath: v3/REST/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  message{id}:
    get:
      summary: Message Detail
      description: View the details of a message.
      operationId: getMessage
      x-api-path-slug: messageid-get
      parameters:
      - in: path
        name: id
        description: Message ID
      responses:
        200:
          description: OK
      tags:
      - Message
      - Detail