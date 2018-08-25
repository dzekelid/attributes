---
swagger: "2.0"
x-collection-name: HERE
x-complete: 0
info:
  title: HERE Route Match Extension API Available Attributes
  description: "*Request which map data layers contain which attributes*\n\nTo make
    a request for map data layer information, use the `attributes``.json` endpoint,
    supplying the `release` and `region` parameters.\n  \n\n\n\n* **region**  `text`\n
    \\- Map Coverage Region.    e.g. `APAC`, `NA`, `EU`\n\n* **release**  `text`\n
    \\- Map release quarter    e.g. `2014Q4` or `LATEST`\n\n* **app_id**  `text`\n
    \\- A 20 byte Base64 URL-safe encoded string used for the authentication of the
    client application.    You must include an `app_id` with every request.\n\n* **app_code**
    \ `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication
    of the client application.    You must include an `app_code` with every request."
  version: 1.0.0
host: pde.cit.api.here.com
basePath: /1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /doc/attributes.json:
    get:
      summary: Available Attributes
      description: "*Request which map data layers contain which attributes*\n\nTo
        make a request for map data layer information, use the `attributes``.json`
        endpoint, supplying the `release` and `region` parameters.\n  \n\n\n\n* **region**
        \ `text`\n \\- Map Coverage Region.    e.g. `APAC`, `NA`, `EU`\n\n* **release**
        \ `text`\n \\- Map release quarter    e.g. `2014Q4` or `LATEST`\n\n* **app_id**
        \ `text`\n \\- A 20 byte Base64 URL-safe encoded string used for the authentication
        of the client application.    You must include an `app_id` with every request.\n\n*
        **app_code**  `text`\n \\- A 20 byte Base64 URL-safe encoded string used for
        the authentication of the client application.    You must include an `app_code`
        with every request."
      operationId: DocAttributesJsonGet
      x-api-path-slug: docattributes-json-get
      parameters:
      - in: query
        name: app_code
      - in: query
        name: app_id
      - in: query
        name: region
      - in: query
        name: release
      responses:
        200:
          description: OK
      tags:
      - Available
      - Attributes
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