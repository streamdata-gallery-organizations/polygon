---
swagger: "2.0"
x-collection-name: Polygon
x-complete: 0
info:
  title: Point-In-Polygon Census Intersection Available Currencies
  description: Get a list of the currencies that polygon.io streams.
  version: 1.0.0
host: api.polygon.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/companies:
    get:
      summary: Available Companies
      description: Get a list of the traded companies that polygon.io streams. Company
        includes some details about the company which we hope to add more to soon.
      operationId: v1.companies.get
      x-api-path-slug: v1companies-get
      parameters:
      - in: query
        name: page
        description: Which page of results to return
      - in: query
        name: perpage
        description: How many items to be on each page during pagination
      - in: query
        name: sort
        description: Which field to sort by
      responses:
        200:
          description: OK
      tags:
      - ""
  /v1/currencies:
    get:
      summary: Available Currencies
      description: Get a list of the currencies that polygon.io streams.
      operationId: v1.currencies.get
      x-api-path-slug: v1currencies-get
      responses:
        200:
          description: OK
      tags:
      - ""
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