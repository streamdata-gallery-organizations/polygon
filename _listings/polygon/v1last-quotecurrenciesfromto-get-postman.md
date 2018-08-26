{
  "info": {
    "name": "Point-In-Polygon Census Intersection Last Quote for a Currency Pair",
    "_postman_id": "ac82d266-9a23-41a2-b44c-b596ab2c63e2",
    "description": "Get Last Quote Tick for a Currency Pair.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "030e8e59-ea50-44bd-bb8e-2ca60ef23c9d",
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
          "id": "7f3898c0-c44a-4e88-b79a-8ccfc0b6effc"
        }
      ]
    },
    {
      "id": "77115651-92c9-46f0-9355-f4ef88fa41d3",
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
          "id": "b409bca2-d9b1-42f1-b7ed-e0efc61d9699"
        }
      ]
    },
    {
      "id": "484d0334-72d7-4b7b-88c8-3f8fa4844d1f",
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
          "id": "be2f4fa4-6dd8-4a01-8214-079d140d9e48"
        }
      ]
    },
    {
      "id": "6b4fe724-a4cd-46ff-b3b7-d60e3b763df8",
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
          "id": "a88429a9-fe82-4ace-9b77-4171d80bdbe1"
        }
      ]
    },
    {
      "id": "50c70709-c4f9-43cf-91c8-374ea37f3840",
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
          "id": "4ca7bbe6-2093-42b9-a1d5-07d7904f2b84"
        }
      ]
    },
    {
      "id": "6465b993-ad33-4895-bb5d-6c1f1bad8b1b",
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
          "id": "e812df5b-e723-491f-b63d-6fb6332c8781"
        }
      ]
    },
    {
      "id": "8949c9a6-8ae2-45bc-8991-e3e34981bcb9",
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
          "id": "3c21dfbd-6bc1-4fbf-aec9-f73c7165d584"
        }
      ]
    },
    {
      "id": "9be6132e-7b43-457c-adf7-ff2d32c3ccb0",
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
          "id": "1e63f5ac-9d3f-4491-b4dd-d95aeebc9eae"
        }
      ]
    },
    {
      "id": "43a417ed-279b-4531-a675-c7fb2b4b6d76",
      "name": "v1.last_quote.currencies.from.to.get",
      "request": {
        "url": {
          "protocol": "http",
          "host": "api.polygon.io",
          "path": [
            "v1/last_quote/currencies/:from/:to"
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
        "description": "Get Last Quote Tick for a Currency Pair."
      },
      "response": [
        {
          "status": "OK",
          "code": 200,
          "name": "Response_200",
          "id": "dbeb4f77-e37e-4f9b-a202-a4573b3b821d"
        }
      ]
    }
  ]
}