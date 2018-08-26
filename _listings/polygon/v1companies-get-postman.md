{
  "info": {
    "name": "Point-In-Polygon Census Intersection Available Companies",
    "_postman_id": "ea30c7f7-6b6a-45a2-a413-a21b53e1512d",
    "description": "Get a list of the traded companies that polygon.io streams. Company includes some details about the company which we hope to add more to soon.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "id": "19fdd220-e155-41a4-9cf6-210fceda5a23",
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
          "id": "872c4457-5270-4723-a43b-e8b78c20b618"
        }
      ]
    }
  ]
}