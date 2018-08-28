swagger: "2.0"
x-collection-name: Lykke
x-complete: 1
info:
  title: Wallet_Api
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/ServerTime:
    get:
      summary: Get API Servertime
      description: Get api servertime.
      operationId: ApiServerTimeGet
      x-api-path-slug: apiservertime-get
      responses:
        200:
          description: OK
      tags:
      - Servertime