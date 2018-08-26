{
  "info": {
    "name": "Point-In-Polygon Census Intersection Last Trade for a Symbol",
    "_postman_id": "09bd1de0-7119-4315-896c-70d926be2531",
    "description": "Get the last trade for a given stock.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "40764056-974e-4447-a7c2-ba49d4a0d227",
      "name": "v1.companies.get",
      "request": {
        "url": "http://api.polygon.io/v1/companies?page=%7B%7D&perpage=%7B%7D&sort=%7B%7D",
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Get a list of the traded companies that polygon.io streams. Company includes some details about the company which we hope to add more to soon."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "fadc902b-f955-4ec5-991f-b5cbab048d7d"
        }
      ]
    },
    {
      "id": "afd85341-9a8b-4bc4-82c0-171aec2bd29f",
      "name": "v1.currencies.get",
      "request": {
        "url": "http://api.polygon.io/v1/currencies",
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Get a list of the currencies that polygon.io streams."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "2fa60074-f6ad-4639-94fb-94c15be98d97"
        }
      ]
    },
    {
      "id": "2e0b4bd9-0d0f-4460-8288-2664ebc67ea7",
      "name": "v1.historic.agg.size.symbol.date.get",
      "request": {
        "url": {
          "protocol": "http",
          "host": "api.polygon.io",
          "path": [
            "v1/historic/agg/:size/:symbol/:date"
          ],
          "query": [
            {
              "key": "limit",
              "value": "%7B%7D",
              "disabled": false
            },
            {
              "key": "offset",
              "value": "%7B%7D",
              "disabled": false
            }
          ],
          "variable": [
            {
              "id": "date",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "size",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "symbol",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Get historic aggregations for a symbol."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "e2a806bc-bf7c-48ad-8df1-34a0bcc5658d"
        }
      ]
    },
    {
      "id": "20bb2f78-88fd-401c-99d8-802c2ba91448",
      "name": "v1.historic.forex.from.to.date.get",
      "request": {
        "url": {
          "protocol": "http",
          "host": "api.polygon.io",
          "path": [
            "v1/historic/forex/:from/:to/:date"
          ],
          "query": [
            {
              "key": "limit",
              "value": "%7B%7D",
              "disabled": false
            },
            {
              "key": "offset",
              "value": "%7B%7D",
              "disabled": false
            }
          ],
          "variable": [
            {
              "id": "date",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "from",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "to",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Get historic ticks for a currency pair. Example for **USD/JPY** the from would be **USD** and to would be **JPY**. The date formatted like **2017-6-22**"
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "a62a1f15-cd5a-436d-8cf5-b19d742b1d2c"
        }
      ]
    },
    {
      "id": "afc761fa-2029-4af3-ac8a-44f320cc736b",
      "name": "v1.historic.quotes.symbol.date.get",
      "request": {
        "url": {
          "protocol": "http",
          "host": "api.polygon.io",
          "path": [
            "v1/historic/quotes/:symbol/:date"
          ],
          "query": [
            {
              "key": "limit",
              "value": "%7B%7D",
              "disabled": false
            },
            {
              "key": "offset",
              "value": "%7B%7D",
              "disabled": false
            }
          ],
          "variable": [
            {
              "id": "date",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "symbol",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Get historic quotes for a symbol."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "7d59513e-007a-453b-913b-ab3f9e9d06da"
        }
      ]
    },
    {
      "id": "3ac1fce9-d8c8-40fe-bc2b-38ed7ca0c3c1",
      "name": "v1.historic.trades.symbol.date.get",
      "request": {
        "url": {
          "protocol": "http",
          "host": "api.polygon.io",
          "path": [
            "v1/historic/trades/:symbol/:date"
          ],
          "query": [
            {
              "key": "limit",
              "value": "%7B%7D",
              "disabled": false
            },
            {
              "key": "offset",
              "value": "%7B%7D",
              "disabled": false
            }
          ],
          "variable": [
            {
              "id": "date",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "symbol",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Get historic trades for a symbol."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "543234a7-2024-4cb7-a596-aad83b694c6b"
        }
      ]
    },
    {
      "id": "07a67d13-6dbf-4122-8e99-59371c8d2125",
      "name": "v1.last.currencies.from.to.get",
      "request": {
        "url": {
          "protocol": "http",
          "host": "api.polygon.io",
          "path": [
            "v1/last/currencies/:from/:to"
          ],
          "variable": [
            {
              "id": "from",
              "value": "{}",
              "type": "string"
            },
            {
              "id": "to",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Get Last Trade Tick for a Currency Pair."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "c9f2c5b2-a4d1-400b-9ad3-ac94060ca158"
        }
      ]
    },
    {
      "id": "a79c6c60-49a5-438e-925c-dfec562b9115",
      "name": "v1.last.stocks.symbol.get",
      "request": {
        "url": {
          "protocol": "http",
          "host": "api.polygon.io",
          "path": [
            "v1/last/stocks/:symbol"
          ],
          "variable": [
            {
              "id": "symbol",
              "value": "{}",
              "type": "string"
            }
          ]
        },
        "method": "GET",
        "header": [
          {
            "key": "Accept",
            "value": "*/*",
            "disabled": false
          }
        ],
        "body": {
          "mode": "raw"
        },
        "description": "Get the last trade for a given stock."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "9573cf64-0d07-4a75-80c8-baf156ae5fb9"
        }
      ]
    }
  ]
}