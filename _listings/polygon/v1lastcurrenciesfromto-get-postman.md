{
  "info": {
    "name": "Point-In-Polygon Census Intersection Last Trade for a Currency Pair",
    "_postman_id": "fed921d9-d7df-4795-8e10-279699b30cbf",
    "description": "Get Last Trade Tick for a Currency Pair.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "f6aeca30-b7e4-4c21-ae88-dd92352911c4",
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
          "id": "fff09e8e-46ad-4f24-b267-71df6dd211ae"
        }
      ]
    },
    {
      "id": "6485a267-ce85-4d02-9518-b64517123b44",
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
          "id": "8e73c080-4b3a-4e7b-a2dc-b3c63d2dfe25"
        }
      ]
    },
    {
      "id": "b4062f3f-6df3-4105-9985-ef8a30b1206e",
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
          "id": "044c9f8c-5e39-40e8-924d-f7a3fe961f58"
        }
      ]
    },
    {
      "id": "abf32439-02bd-4137-9e43-1463a22a5c26",
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
          "id": "b0b593fd-e360-4e4f-b3bc-dc34cc403d08"
        }
      ]
    },
    {
      "id": "1764d2d7-9f10-47d8-8e89-7970f6f78214",
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
          "id": "7ca64b79-e034-4a32-8548-8ac847b4a647"
        }
      ]
    },
    {
      "id": "13bf3188-2c19-4ab3-9206-cd0626755219",
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
          "id": "fa4dd312-8512-4272-ab87-073010689a10"
        }
      ]
    },
    {
      "id": "2aa99274-9adb-432d-857b-1ef0b4fa8b58",
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
          "id": "79029e7d-f159-410a-84c6-844718481315"
        }
      ]
    }
  ]
}