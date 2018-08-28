swagger: "2.0"
x-collection-name: AWS Elastic Beanstalk
x-complete: 1
info:
  title: AWS Elastic Beanstalk API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=RestartAppServer:
    get:
      summary: Restart App Server
      description: |-
        Causes the environment to restart the application container server running on each
              Amazon EC2 instance.
      operationId: restartAppServer
      x-api-path-slug: actionrestartappserver-get
      parameters:
      - in: query
        name: EnvironmentId
        description: The ID of the environment to restart the server for
        type: string
      - in: query
        name: EnvironmentName
        description: The name of the environment to restart the server for
        type: string
      responses:
        200:
          description: OK
      tags:
      - App Servers