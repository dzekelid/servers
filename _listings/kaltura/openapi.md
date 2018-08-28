swagger: "2.0"
x-collection-name: Kaltura
x-complete: 1
info:
  title: Kaltura VPaaS
  description: building-video-experiences-consists-of-ingesting-media-files-playing-back-videos-and-reviewing-usage-and-engagement-analytics--in-between-there-is-a-world-of-nuances-required-for-your-unique-usecase-and-application--kaltura-vpaas-is-built-on-the-principles-of-atomic-services-sdks-and-tools-that-allow-you-full-control-and-flexibility-over-every-element-and-process-in-your-medias-life-cycle-
  version: 3.3.0
host: www.kaltura.com
basePath: /api_v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /service/contentdistribution_entrydistribution/action/serveReturnedData:
    get:
      summary: Get Service Contentdistribution Entrydistribution Action Servereturneddata
      description: Serves entry distribution returned data
      operationId: entryDistribution.serveReturnedData
      x-api-path-slug: servicecontentdistribution-entrydistributionactionservereturneddata-get
      parameters:
      - in: query
        name: actionType
        description: 'Enum Type: `KalturaDistributionAction`'
      - in: query
        name: id
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Contentdistribution
      - Entrydistribution
      - Action
      - ServeReturnedData