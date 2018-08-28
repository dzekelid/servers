swagger: "2.0"
x-collection-name: Google Container Engine
x-complete: 1
info:
  title: Google Container Engine
  description: builds-and-manages-clusters-that-run-containerbased-applications-powered-by-open-source-kubernetes-technology-
  contact:
    name: Google
    url: https://google.com
  version: v1
host: container.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/projects/{projectId}/zones/{zone}/serverconfig:
    get:
      summary: Get Server Configuration
      description: Returns configuration info about the Container Engine service.
      operationId: container.projects.zones.getServerconfig
      x-api-path-slug: v1projectsprojectidzoneszoneserverconfig-get
      parameters:
      - in: path
        name: projectId
        description: The Google Developers Console [project ID or project number](https://support
      - in: path
        name: zone
        description: The name of the Google Compute Engine [zone](/compute/docs/zones#available)
          to return operations for
      responses:
        200:
          description: OK
      tags:
      - Server