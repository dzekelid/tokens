{
  "info": {
    "name": "Pivotal Tracker Get Tokens Active",
    "_postman_id": "4dc34e1f-669f-4972-bd43-e5ee5a899369",
    "description": "Returns an API token associated with the user. This method requires HTTP Basic authentication.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Tokens",
      "item": [
        {
          "id": "4d4bdf15-c171-4f94-8a57-b8c9a5b757f3",
          "name": "getTokensActive",
          "request": {
            "url": "http://www.pivotaltracker.com/services/v3/tokens/active",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns an API token associated with the user. This method requires HTTP Basic authentication."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "94eb0e9a-6337-414b-b564-63061d6bb101"
            }
          ]
        }
      ]
    }
  ]
}