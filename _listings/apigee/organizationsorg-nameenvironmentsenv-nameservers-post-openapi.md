---
swagger: "2.0"
x-collection-name: Apigee
x-complete: 0
info:
  title: Apigee Edge Post Organizations Name Environments Env Name Servers
  description: Add servers into the environment.
  version: 1.0.0
host: api.enterprise.apigee.com
basePath: /v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /organizations/{org_name}/environments/{env_name}/servers:
    get:
      summary: Get Organizations Name Environments Env Name Servers
      description: Gets the servers that are bound to an environment.
      operationId: getOrganizationsOrgNameEnvironmentsEnvNameServers
      x-api-path-slug: organizationsorg-nameenvironmentsenv-nameservers-get
      parameters:
      - in: path
        name: env_name
        description: Mention the environment name
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Environments
      - Env
      - Servers
    post:
      summary: Post Organizations Name Environments Env Name Servers
      description: Add servers into the environment.
      operationId: postOrganizationsOrgNameEnvironmentsEnvNameServers
      x-api-path-slug: organizationsorg-nameenvironmentsenv-nameservers-post
      parameters:
      - in: path
        name: env_name
        description: Mention the environment name
      - in: path
        name: org_name
        description: Mention the organization name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Environments
      - Env
      - Servers
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