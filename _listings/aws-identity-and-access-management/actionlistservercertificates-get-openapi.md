---
swagger: "2.0"
x-collection-name: AWS Identity and Access Management
x-complete: 0
info:
  title: AWS Identity and Access Management API List Server Certificates
  version: 1.0.0
  description: Lists the server certificates stored in IAM that have the specified
    path prefix.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DeleteServerCertificate:
    get:
      summary: Delete Server Certificate
      description: Deletes the specified server certificate.
      operationId: deleteServerCertificate
      x-api-path-slug: actiondeleteservercertificate-get
      parameters:
      - in: query
        name: ServerCertificateName
        description: The name of the server certificate you want to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Server Certificates
  /?Action=GetServerCertificate:
    get:
      summary: Get Server Certificate
      description: Retrieves information about the specified server certificate stored
        in IAM.
      operationId: getServerCertificate
      x-api-path-slug: actiongetservercertificate-get
      parameters:
      - in: query
        name: ServerCertificateName
        description: The name of the server certificate you want to retrieve information
          about
        type: string
      responses:
        200:
          description: OK
      tags:
      - Server Certificates
  /?Action=ListServerCertificates:
    get:
      summary: List Server Certificates
      description: Lists the server certificates stored in IAM that have the specified
        path prefix.
      operationId: listServerCertificates
      x-api-path-slug: actionlistservercertificates-get
      parameters:
      - in: query
        name: Marker
        description: Use this parameter only when paginating results and only after     you
          receive a response indicating that the results are truncated
        type: string
      - in: query
        name: MaxItems
        description: (Optional) Use this only when paginating results to indicate
          the     maximum number of items you want in the response
        type: string
      - in: query
        name: PathPrefix
        description: The path prefix for filtering the results
        type: string
      responses:
        200:
          description: OK
      tags:
      - Serve rCertificates
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