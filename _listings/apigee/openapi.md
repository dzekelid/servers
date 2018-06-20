---
swagger: "2.0"
x-collection-name: Apigee
x-complete: 1
info:
  title: Apigee Edge
  description: restful-management-api-to-create-configure-and-manage-api-proxies-and-api-products-create-and-manage-apps-and-app-developers-and-more-
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
    delete:
      summary: Delete Organizations Name Environments Env Name Servers
      description: Deletes servers from the environment.
      operationId: deleteOrganizationsOrgNameEnvironmentsEnvNameServers
      x-api-path-slug: organizationsorg-nameenvironmentsenv-nameservers-delete
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
---