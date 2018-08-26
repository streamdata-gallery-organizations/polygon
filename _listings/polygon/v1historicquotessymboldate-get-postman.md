{
  "info": {
    "name": "Point-In-Polygon Census Intersection Historic Quotes",
    "_postman_id": "c218e01c-91c6-430b-8b5d-d3e9694c4646",
    "description": "Get historic quotes for a symbol.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "2c38ef90-3343-49a9-bbea-cb464ad757a7",
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
          "id": "405131c1-3a8f-4bcc-9c7d-dcf79fb8a758"
        }
      ]
    },
    {
      "id": "5b457568-e6ff-4fe2-8912-2b5be532d6f7",
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
          "id": "1cc5fbc9-520c-44fa-b85a-41e16522bf6c"
        }
      ]
    },
    {
      "id": "ac0fe8ea-cdaa-45c4-9630-1d5b6bf67f9b",
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
          "id": "e876b6c6-197e-44bd-b4f1-ca10d9167d22"
        }
      ]
    },
    {
      "id": "b5934b5d-3825-4def-87c4-a8a5bd1aad8b",
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
          "id": "ce78fd7f-459c-4b19-80c0-df6bcda49705"
        }
      ]
    },
    {
      "id": "fdb8cd4a-99bf-4b32-a595-7c919f6366d2",
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
          "id": "6069baf2-5a07-4a1d-8bdc-3352b971391f"
        }
      ]
    }
  ]
}