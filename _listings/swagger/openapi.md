swagger: "2.0"
x-collection-name: Swagger
x-complete: 1
info:
  title: Swagger Generator
  description: this-is-an-online-swagger-codegen-server---you-can-find-out-more-at-httpsgithub-comswaggerapiswaggercodegen-or-on-irc-freenode-net-swaggerhttpswagger-ioirc-
  termsOfService: http://swagger.io/terms/
  contact:
    name: apiteam@swagger.io
  version: 2.2.3
host: generator.swagger.io
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /gen/servers:
    get:
      summary: Gets languages supported by the server generator
      description: Gets languages supported by the server generator.
      operationId: serverOptions
      x-api-path-slug: genservers-get
      responses:
        200:
          description: OK
      tags:
      - Generate
      - Servers
  /gen/servers/{framework}:
    get:
      summary: Returns options for a server framework
      description: Returns options for a server framework.
      operationId: getServerOptions
      x-api-path-slug: genserversframework-get
      parameters:
      - in: path
        name: framework
        description: The target language for the server framework
      responses:
        200:
          description: OK
      tags:
      - Generate
      - Servers
      - Framework
    post:
      summary: Generates a server library
      description: Accepts a `GeneratorInput` options map for spec location and generation
        options.
      operationId: generateServerForLanguage
      x-api-path-slug: genserversframework-post
      parameters:
      - in: body
        name: body
        description: parameters
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: framework
        description: framework
      responses:
        200:
          description: OK
      tags:
      - Generate
      - Servers
      - Framework