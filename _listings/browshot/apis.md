---
name: Browshot
x-slug: browshot
description: Browshot is a service to take screenshot of web pages. Use any of our
  mobile and desktop browsers. We provide a powerful API and libraries.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/717-browshot-com.jpg
x-kinRank: "7"
x-alexaRank: "1714303"
tags: Thumbnails
created: "2018-08-26"
modified: "2018-08-26"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/thumbnails/master/_listings/browshot/apis.md
specificationVersion: "0.14"
apis:
- name: Browshot - Retrieve a thumbnail image
  x-api-slug: screenshotthumbnail-get
  description: |-
    Unlike the other API calls, this API sends back the thumbnail as a PNG file, not JSON. The HTTP response code indicates whether the screenshot was successful (200), or incomplete (404) or failed (404). If the screenshot failed or is not finished, a default image "Not found" is sent.

    You can crop your screenshots. The crop is done first, then the thumbnail. You can take a 1024x768 screenshot, crop it to 768x768, and get it scaled down to 300x300.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/717-browshot-com.jpg
  humanURL: http://browshot.com/
  baseURL: https://api.browshot.com//api/v1
  tags: Browsers, Screenshot, Utility, Screen Capture, Mobile, Technology, SaaS, internet,
    API Provider, Profiles, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/thumbnails/master/_listings/browshot/screenshotthumbnail-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/thumbnails/master/_listings/browshot/screenshotthumbnail-get-openapi.md
- name: Browshot - Retrieve a thumbnail image
  x-api-slug: screenshotthumbnail-get
  description: |-
    Unlike the other API calls, this API sends back the thumbnail as a PNG file, not JSON. The HTTP response code indicates whether the screenshot was successful (200), or incomplete (404) or failed (404). If the screenshot failed or is not finished, a default image "Not found" is sent.

    You can crop your screenshots. The crop is done first, then the thumbnail. You can take a 1024x768 screenshot, crop it to 768x768, and get it scaled down to 300x300.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/717-browshot-com.jpg
  humanURL: http://browshot.com/
  baseURL: https://api.browshot.com//api/v1
  tags: Browsers, Screenshot, Utility, Screen Capture, Mobile, Technology, SaaS, internet,
    API Provider, Profiles, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/thumbnails/master/_listings/browshot/screenshotthumbnail-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/thumbnails/master/_listings/browshot/screenshotthumbnail-get-openapi.md
x-common:
- type: x-website
  url: http://browshot.com/
- type: x-api-gallery
  url: http://broadleaf.commerce.api.gallery.streamdata.io
- type: x-api-stack
  url: http://browshot.stack.network
- type: x-base
  url: https://api.browshot.com/api/
- type: x-blog
  url: http://blog.browshot.com/
- type: x-blog-rss
  url: http://blog.browshot.com/feeds/posts/default
- type: x-crunchbase
  url: http://www.crunchbase.com/company/browshot
- type: x-crunchbase
  url: https://crunchbase.com/organization/browshot
- type: x-developer
  url: http://browshot.com/api/documentation
- type: x-email
  url: feedback@browshot.com
- type: x-twitter
  url: https://twitter.com/BrowshotCom
- type: x-website
  url: http://browshot.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---