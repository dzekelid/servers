---
name: Postmark
x-slug: postmark
description: Trusted by thousands of developers, Postmark is a fast and reliable transactional
  email service. Send with Postmark to ensure your transactional emails get to the
  inbox on time, every time.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
x-kinRank: "8"
x-alexaRank: "87545"
tags: Servers
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/servers/master/_listings/postmark/apis.md
specificationVersion: "0.14"
apis:
- name: Postmark - Parameters Server
  x-api-slug: server-parameters
  description: Parameters server.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://spamcheck.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/servers/master/_listings/postmark/server-parameters-openapi.md
- name: Postmark - Get Server
  x-api-slug: server-get
  description: Gets the server details and figures out your unique InboundHash where
    you can forward your email. This can be found in the web app in your server's
    Credentials tab or via the API.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://spamcheck.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/servers/master/_listings/postmark/server-get-openapi.md
- name: Postmark - Post Server
  x-api-slug: server-post
  description: Sets the URL where we should send JSON data. In order for your application
    receive the emails that we parse, you will need to tell Postmark where to send
    the JSON data for each inbound email it processes, which is done via an HTTP POST
    to a URL of your choice. You can set this URL in the Settings page for your Postmark
    server in the web app, or using the InboundHookUrl field in the API. It also lets
    you choose a domain that you would like to listen on for incoming email to be
    processed by Postmark. We recommend a separate subdomain, like inbound.yourdomain.com.
    Each server can listen to one unique domain, so make sure to set the X-Postmark-Server-Token
    to the correct server token in the API call below.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://spamcheck.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/servers/master/_listings/postmark/server-post-openapi.md
- name: Postmark - Put Server
  x-api-slug: server-put
  description: Put server.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://spamcheck.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/servers/master/_listings/postmark/server-put-openapi.md
- name: Postmark - Parameters Server
  x-api-slug: server-parameters
  description: Parameters server.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://spamcheck.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/servers/master/_listings/postmark/server-parameters-openapi.md
- name: Postmark - Get Server
  x-api-slug: server-get
  description: Gets the server details and figures out your unique InboundHash where
    you can forward your email. This can be found in the web app in your server's
    Credentials tab or via the API.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://spamcheck.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/servers/master/_listings/postmark/server-get-openapi.md
- name: Postmark - Post Server
  x-api-slug: server-post
  description: Sets the URL where we should send JSON data. In order for your application
    receive the emails that we parse, you will need to tell Postmark where to send
    the JSON data for each inbound email it processes, which is done via an HTTP POST
    to a URL of your choice. You can set this URL in the Settings page for your Postmark
    server in the web app, or using the InboundHookUrl field in the API. It also lets
    you choose a domain that you would like to listen on for incoming email to be
    processed by Postmark. We recommend a separate subdomain, like inbound.yourdomain.com.
    Each server can listen to one unique domain, so make sure to set the X-Postmark-Server-Token
    to the correct server token in the API call below.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://spamcheck.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/servers/master/_listings/postmark/server-post-openapi.md
- name: Postmark - Put Server
  x-api-slug: server-put
  description: Put server.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://spamcheck.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/servers/master/_listings/postmark/server-put-openapi.md
- name: Postmark - Put Server
  x-api-slug: server-put
  description: Put server.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://spamcheck.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/servers/master/_listings/postmark/server-put-openapi.md
- name: Postmark - Post Server
  x-api-slug: server-post
  description: Sets the URL where we should send JSON data. In order for your application
    receive the emails that we parse, you will need to tell Postmark where to send
    the JSON data for each inbound email it processes, which is done via an HTTP POST
    to a URL of your choice. You can set this URL in the Settings page for your Postmark
    server in the web app, or using the InboundHookUrl field in the API. It also lets
    you choose a domain that you would like to listen on for incoming email to be
    processed by Postmark. We recommend a separate subdomain, like inbound.yourdomain.com.
    Each server can listen to one unique domain, so make sure to set the X-Postmark-Server-Token
    to the correct server token in the API call below.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://spamcheck.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/servers/master/_listings/postmark/server-post-openapi.md
- name: Postmark - Get Server
  x-api-slug: server-get
  description: Gets the server details and figures out your unique InboundHash where
    you can forward your email. This can be found in the web app in your server's
    Credentials tab or via the API.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://spamcheck.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/servers/master/_listings/postmark/server-get-openapi.md
- name: Postmark - Parameters Server
  x-api-slug: server-parameters
  description: Parameters server.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://spamcheck.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/servers/master/_listings/postmark/server-parameters-openapi.md
- name: Postmark Account-level - List servers
  x-api-slug: servers-get
  description: List servers.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://api.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/servers/master/_listings/postmark/servers-get-openapi.md
- name: Postmark Account-level - Create a Server
  x-api-slug: servers-post
  description: Create a server.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://api.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/servers/master/_listings/postmark/servers-post-openapi.md
- name: Postmark Account-level - Delete a Server
  x-api-slug: serversserverid-delete
  description: Delete a server.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://api.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/servers/master/_listings/postmark/serversserverid-delete-openapi.md
- name: Postmark Account-level - Get a Server
  x-api-slug: serversserverid-get
  description: Get a server.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://api.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/servers/master/_listings/postmark/serversserverid-get-openapi.md
- name: Postmark Account-level - Edit a Server
  x-api-slug: serversserverid-put
  description: Edit a server.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://api.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/servers/master/_listings/postmark/serversserverid-put-openapi.md
- name: Postmark Account-level - Delete a Server
  x-api-slug: serversserverid-delete
  description: Delete a server.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://api.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/servers/master/_listings/postmark/serversserverid-delete-openapi.md
- name: Postmark Account-level - Get a Server
  x-api-slug: serversserverid-get
  description: Get a server.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://api.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/servers/master/_listings/postmark/serversserverid-get-openapi.md
- name: Postmark Account-level - Edit a Server
  x-api-slug: serversserverid-put
  description: Edit a server.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://api.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/servers/master/_listings/postmark/serversserverid-put-openapi.md
- name: Postmark Account-level - Delete a Server
  x-api-slug: serversserverid-delete
  description: Delete a server.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://api.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/servers/master/_listings/postmark/serversserverid-delete-openapi.md
- name: Postmark Account-level - Get a Server
  x-api-slug: serversserverid-get
  description: Get a server.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://api.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/servers/master/_listings/postmark/serversserverid-get-openapi.md
- name: Postmark Account-level - Edit a Server
  x-api-slug: serversserverid-put
  description: Edit a server.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://api.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/servers/master/_listings/postmark/serversserverid-put-openapi.md
- name: Postmark Account-level - Edit a Server
  x-api-slug: serversserverid-put
  description: Edit a server.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://api.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/servers/master/_listings/postmark/serversserverid-put-openapi.md
- name: Postmark Account-level - Get a Server
  x-api-slug: serversserverid-get
  description: Get a server.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://api.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/servers/master/_listings/postmark/serversserverid-get-openapi.md
- name: Postmark Account-level - Delete a Server
  x-api-slug: serversserverid-delete
  description: Delete a server.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/638-postmark.jpg
  humanURL: http://postmarkapp.com
  baseURL: https://api.postmarkapp.com//
  tags: Target, Imports, Stack Network, Technology, SaaS, Emails, Messages, Relative
    Data, Service API, Relative StreamRank, Streams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/servers/master/_listings/postmark/serversserverid-delete-openapi.md
x-common:
- type: x--net-library
  url: http://developer.postmarkapp.com/developer-official-libs.html#dot-net
- type: x-api-gallery
  url: http://polygon.api.gallery.streamdata.io
- type: x-api-stack
  url: http://postmark.stack.network
- type: x-base
  url: https://api.postmarkapp.com
- type: x-blog
  url: http://blog.postmarkapp.com/
- type: x-blog-rss
  url: http://blog.postmarkapp.com/rss
- type: x-contact-form
  url: http://support.postmarkapp.com/customer/portal/emails/new
- type: x-crunchbase
  url: https://crunchbase.com/organization/postmark
- type: x-crunchbase
  url: http://www.crunchbase.com/company/postmark
- type: x-developer
  url: http://developer.postmarkapp.com/
- type: x-email
  url: support@postmarkapp.com
- type: x-email
  url: 451d9b70cf9364d23ff6f9d51d870251569e+ahoy@inbound.postmarkapp.com
- type: x-faq
  url: http://support.postmarkapp.com/
- type: x-pricing
  url: http://developer.postmarkapp.com/developer-api-messages.html
- type: x-privacy
  url: https://postmarkapp.com/privacy-policy
- type: x-ruby-library
  url: http://developer.postmarkapp.com/developer-official-libs.html#rails
- type: x-ruby-library
  url: http://developer.postmarkapp.com/developer-official-libs.html#ruby
- type: x-selfservice-registration
  url: https://postmarkapp.com/sign_up
- type: x-status
  url: http://status.postmarkapp.com/
- type: x-terms-of-service
  url: https://postmarkapp.com/terms-of-service
- type: x-twitter
  url: https://twitter.com/postmarkapp
- type: x-website
  url: http://postmarkapp.com
- type: x-website
  url: http://postmarkapp.com/
- type: x-website
  url: https://postmarkapp.com
- type: x-wordpress-pdk
  url: http://developer.postmarkapp.com/developer-official-libs.html#wordpress
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---