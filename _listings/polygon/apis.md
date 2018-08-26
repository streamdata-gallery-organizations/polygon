---
name: Polygon
x-slug: polygon
description: Polygon.io offers streaming realtime data for stocks/equities, ETFs,
  Indecies and Forex/Currencies including crypto currencies. Our Real-Time Stock Data
  APIs help you build the future on fintech.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/polygon-logo.png
x-kinRank: "7"
x-alexaRank: "2931123"
tags: Polygon
created: "2018-08-26"
modified: "2018-08-26"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/polygon/master/_listings/polygon/apis.md
specificationVersion: "0.14"
apis:
- name: Polygon - Available Companies
  x-api-slug: v1companies-get
  description: Get a list of the traded companies that polygon.io streams. Company
    includes some details about the company which we hope to add more to soon.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/polygon-logo.png
  humanURL: http://polygon.io
  baseURL: https://api.polygon.io//
  tags: Financial, Market Data, General Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/polygon/master/_listings/polygon/v1companies-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/polygon/master/_listings/polygon/v1companies-get-openapi.md
- name: Polygon - Available Currencies
  x-api-slug: v1currencies-get
  description: Get a list of the currencies that polygon.io streams.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/polygon-logo.png
  humanURL: http://polygon.io
  baseURL: https://api.polygon.io//
  tags: Financial, Market Data, General Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/polygon/master/_listings/polygon/v1currencies-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/polygon/master/_listings/polygon/v1currencies-get-openapi.md
- name: Polygon - Historic Aggregates
  x-api-slug: v1historicaggsizesymboldate-get
  description: Get historic aggregations for a symbol.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/polygon-logo.png
  humanURL: http://polygon.io
  baseURL: https://api.polygon.io//
  tags: Financial, Market Data, General Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/polygon/master/_listings/polygon/v1historicaggsizesymboldate-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/polygon/master/_listings/polygon/v1historicaggsizesymboldate-get-openapi.md
- name: Polygon - Historic Forex Ticks
  x-api-slug: v1historicforexfromtodate-get
  description: Get historic ticks for a currency pair. Example for **USD/JPY** the
    from would be **USD** and to would be **JPY**. The date formatted like **2017-6-22**
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/polygon-logo.png
  humanURL: http://polygon.io
  baseURL: https://api.polygon.io//
  tags: Financial, Market Data, General Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/polygon/master/_listings/polygon/v1historicforexfromtodate-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/polygon/master/_listings/polygon/v1historicforexfromtodate-get-openapi.md
- name: Polygon - Historic Quotes
  x-api-slug: v1historicquotessymboldate-get
  description: Get historic quotes for a symbol.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/polygon-logo.png
  humanURL: http://polygon.io
  baseURL: https://api.polygon.io//
  tags: Financial, Market Data, General Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/polygon/master/_listings/polygon/v1historicquotessymboldate-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/polygon/master/_listings/polygon/v1historicquotessymboldate-get-openapi.md
- name: Polygon - Historic Trades
  x-api-slug: v1historictradessymboldate-get
  description: Get historic trades for a symbol.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/polygon-logo.png
  humanURL: http://polygon.io
  baseURL: https://api.polygon.io//
  tags: Financial, Market Data, General Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/polygon/master/_listings/polygon/v1historictradessymboldate-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/polygon/master/_listings/polygon/v1historictradessymboldate-get-openapi.md
- name: Polygon - Last Trade for a Currency Pair
  x-api-slug: v1lastcurrenciesfromto-get
  description: Get Last Trade Tick for a Currency Pair.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/polygon-logo.png
  humanURL: http://polygon.io
  baseURL: https://api.polygon.io//
  tags: Financial, Market Data, General Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/polygon/master/_listings/polygon/v1lastcurrenciesfromto-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/polygon/master/_listings/polygon/v1lastcurrenciesfromto-get-openapi.md
- name: Polygon - Last Trade for a Symbol
  x-api-slug: v1laststockssymbol-get
  description: Get the last trade for a given stock.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/polygon-logo.png
  humanURL: http://polygon.io
  baseURL: https://api.polygon.io//
  tags: Financial, Market Data, General Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/polygon/master/_listings/polygon/v1laststockssymbol-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/polygon/master/_listings/polygon/v1laststockssymbol-get-openapi.md
- name: Polygon - Last Quote for a Currency Pair
  x-api-slug: v1last-quotecurrenciesfromto-get
  description: Get Last Quote Tick for a Currency Pair.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/polygon-logo.png
  humanURL: http://polygon.io
  baseURL: https://api.polygon.io//
  tags: Financial, Market Data, General Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/polygon/master/_listings/polygon/v1last-quotecurrenciesfromto-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/polygon/master/_listings/polygon/v1last-quotecurrenciesfromto-get-openapi.md
- name: Polygon - Last Quote for a Symbol
  x-api-slug: v1last-quotestockssymbol-get
  description: Get the last quote tick for a given stock.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/polygon-logo.png
  humanURL: http://polygon.io
  baseURL: https://api.polygon.io//
  tags: Financial, Market Data, General Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/polygon/master/_listings/polygon/v1last-quotestockssymbol-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/polygon/master/_listings/polygon/v1last-quotestockssymbol-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://plivo.api.gallery.streamdata.io
- type: x-api-stack
  url: http://polygon.stack.network
- type: x-blog
  url: https://polygon.io/blog/
- type: x-blog-rss
  url: https://polygon.io/blog/rss/
- type: x-documentation
  url: https://polygon.io/docs/#getting-started
- type: x-github
  url: https://github.com/polygon-io
- type: x-selfservice-registration
  url: https://polygon.io/signup
- type: x-twitter
  url: https://twitter.com/polygon_io
- type: x-website
  url: http://polygon.io
- type: x-website
  url: https://polygon.io
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---