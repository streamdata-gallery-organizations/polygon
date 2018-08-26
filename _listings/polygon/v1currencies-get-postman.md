{
  "info": {
    "name": "Point-In-Polygon Census Intersection Available Currencies",
    "_postman_id": "cf9f189e-8fb6-4ac0-ba11-6f514aa29eb0",
    "description": "Get a list of the currencies that polygon.io streams.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "c4a291a1-3cab-4ef7-a8ba-01af2d3b8e6a",
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
          "id": "ee4c7a6c-e194-4a5f-b2b0-c4bd1cb11536"
        }
      ]
    },
    {
      "id": "faa01ede-f7e7-4919-bfff-cf48d3daa2e0",
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
          "id": "87366f3b-f33d-4551-980f-6cf95cb0dda5"
        }
      ]
    }
  ]
}