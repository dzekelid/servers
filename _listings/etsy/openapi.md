swagger: "2.0"
x-collection-name: Etsy
x-complete: 1
info:
  title: Etsy
  description: bring-etsys-handmade-marketplace-and-community-into-your-apps-
  version: 1.0.0
host: openapi.etsy.com
basePath: /v2/private/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /server/epoch:
    get:
      summary: Get Server Epoch
      description: Get server time, in epoch seconds notation.
      operationId: getServerEpoch
      x-api-path-slug: serverepoch-get
      responses:
        200:
          description: OK
      tags:
      - Server
      - Epoch
  /server/ping:
    get:
      summary: Get Server Ping
      description: Check that the server is alive.
      operationId: getServerPing
      x-api-path-slug: serverping-get
      responses:
        200:
          description: OK
      tags:
      - Server
      - Ping