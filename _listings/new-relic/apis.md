---
name: New Relic
x-slug: new-relic
description: New Relic???s digital intelligence platform lets developers, ops, and
  tech teams measure and monitor the performance of their applications and infrastructure.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
x-kinRank: "8"
x-alexaRank: "10322"
tags: Servers
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/servers/master/_listings/new-relic/apis.md
specificationVersion: "0.14"
apis:
- name: New Relic Get Servers. Format
  x-api-slug: new-relic
  description: |-
    This API endpoint returns a paginated
    list of the Servers associated with your New Relic account. The time range for summary data is the last 10 minutes.

    Servers can be filtered by their name, hostname, or the list of server IDs.

    See our documentation for a discussion and examples of
    using filters
    and summary data output.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///servers.{format}
  tags: Servers., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/servers/master/_listings/new-relic/servers-format-get-openapi.md
- name: New Relic Get Servers  . Format
  x-api-slug: new-relic
  description: "This API endpoint returns a single Server, identified by ID. The time
    range for summary data is the last 10 minutes.\u201D\n\nSee our documentation
    for a discussion on\nsummary data output."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///servers/{id}.{format}
  tags: Servers, , ., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/servers/master/_listings/new-relic/serversid-format-get-openapi.md
- name: New Relic Put Servers  . Format
  x-api-slug: new-relic
  description: |-
    This API endpoint allows you to rename your server.

    The input is expected to be in JSON or XML format in the body parameter of the PUT request. The exact
    schema is defined below. Any extra parameters passed in the body will be ignored.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///servers/{id}.{format}
  tags: Servers, , ., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/servers/master/_listings/new-relic/serversid-format-put-openapi.md
- name: New Relic Delete Servers  . Format
  x-api-slug: new-relic
  description: |-
    This API endpoint deletes a server and all of its reported data.

    WARNING: Only servers that have stopped reporting can be deleted. This is an irreversible process which
    will delete all reported data for this server.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///servers/{id}.{format}
  tags: Servers, , ., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/servers/master/_listings/new-relic/serversid-format-delete-openapi.md
- name: New Relic Get Servers Server  Metrics. Format
  x-api-slug: new-relic
  description: |-
    Return a list of known metrics and their value names for the given resource.

    See our documentation for a discussion
    on  output pagination
    and for examples of requesting and using metric values.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///servers/{server_id}/metrics.{format}
  tags: Servers, Server, , Metrics., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/servers/master/_listings/new-relic/serversserver-idmetrics-format-get-openapi.md
- name: New Relic Get Servers Server  Metrics Data. Format
  x-api-slug: new-relic
  description: "This API endpoint returns a list of values for each of the requested
    metrics. The list of available metrics\ncan be returned using the Metric Name
    API endpoint.\n\nMetric data can be filtered by a number of parameters, including
    multiple names and values, and by time range.\nMetric names and values will be
    matched intelligently in the background.\n\nYou can also retrieve a summarized
    data point across the entire time range selected by using the summarize\nparameter.\n\nSee
    our documentation for a discussion on \noutput pagination,  time range \nrelated
    considerations, and for examples of requesting and using metric values."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2///servers/{server_id}/metrics/data.{format}
  tags: Servers, Server, , Metrics, Data., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/servers/master/_listings/new-relic/serversserver-idmetricsdata-format-get-openapi.md
- name: New Relic
  x-api-slug: new-relic
  description: New Relic???s digital intelligence platform lets developers, ops, and
    tech teams measure and monitor the performance of their applications and infrastructure.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2/
  tags: Servers
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/servers/master/_listings/new-relic/openapi.md
x-common:
- type: x-blog
  url: https://blog.newrelic.com/
- type: x-blog-rss
  url: https://blog.newrelic.com/feed/
- type: x-crunchbase
  url: https://crunchbase.com/organization/new-relic
- type: x-developer
  url: https://rpm.newrelic.com/api/explore/
- type: x-email
  url: billing@newrelic.com
- type: x-email
  url: resume@newrelic.com
- type: x-email
  url: PR@newrelic.com
- type: x-email
  url: copyright@newrelic.com
- type: x-email
  url: dataprivacy@newrelic.com
- type: x-email
  url: PersonalDataRequest@newrelic.com
- type: x-email
  url: support@newrelic.com
- type: x-email
  url: compliance@newrelic.com
- type: x-github
  url: https://github.com/newrelic
- type: x-twitter
  url: https://twitter.com/NewRelic
- type: x-website
  url: https://newrelic.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---