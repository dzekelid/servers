---
name: Hewlett Packard Enterprise (HPE)
x-slug: hewlett-packard-enterprise-hpe
description: We help customers use technology to slash the time it takes to turn ideas
  into value. In turn, they transform industries, markets and lives. Some of our customers
  run traditional IT environments. Most are transitioning to a secure, cloud-enabled,
  mobile-friendly infrastructure. Many rely on a combination of both. Wherever they
  are in that journey, we provide the technology and solutions to help them succeed.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
x-kinRank: "8"
x-alexaRank: "0"
tags: Servers
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/servers/master/_listings/hewlett-packard-enterprise-hpe/apis.md
specificationVersion: "0.14"
apis:
- name: HPE OneSphere API - Get Servers
  x-api-slug: servers-get
  description: Returns servers.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/servers/master/_listings/hewlett-packard-enterprise-hpe/servers-get-openapi.md
- name: HPE OneSphere API - Post Servers
  x-api-slug: servers-post
  description: Create/Register a server.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/servers/master/_listings/hewlett-packard-enterprise-hpe/servers-post-openapi.md
- name: HPE OneSphere API - Delete Servers
  x-api-slug: serversid-delete
  description: |-
    Delete a server.
    Note that by default only servers created via the HPE OneSphere API can be
    subsequently deleted. HPE OneSphere managed servers (those that have
    an applianceUri) cannot be deleted via this operation (a '403' will be returned),
    unless the 'force' parameter is supplied and set to 'true'.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/servers/master/_listings/hewlett-packard-enterprise-hpe/serversid-delete-openapi.md
- name: HPE OneSphere API - Get Servers
  x-api-slug: serversid-get
  description: Returns a server based on its ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/servers/master/_listings/hewlett-packard-enterprise-hpe/serversid-get-openapi.md
- name: HPE OneSphere API - Patch Servers
  x-api-slug: serversid-patch
  description: Update properties of a server.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/HPE-logo.png
  humanURL: http://HPE.com
  baseURL: https://deic02-hpe.hpeonesphere.com//rest
  tags: Enterprise, Cloud, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/servers/master/_listings/hewlett-packard-enterprise-hpe/serversid-patch-openapi.md
x-common:
- type: x-developer
  url: https://developer.hpe.com/
- type: x-github
  url: https://github.com/hewlettpackard
- type: x-openapi
  url: https://raw.githubusercontent.com/HewlettPackard/hpe-onesphere-http/master/swagger.yml
- type: x-twitter
  url: https://twitter.com/HPE
- type: x-website
  url: http://HPE.com
- type: x-api-gallery
  url: http://heroku.api.gallery.streamdata.io
- type: x-api-stack
  url: http://hewlett.packard.enterprise.hpe.stack.network
- type: x-blog
  url: https://developer.hpe.com/blog
- type: x-curated-source
  url: http://community.hpe.com/t5/LoadRunner-and-Performance/LoadRunner-and-VuGen-12-53-load-testing-software-What-s-new-in/ba-p/6885101
- type: x-website
  url: https://www.hpe.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---