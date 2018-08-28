{
  "info": {
    "name": "Bitly Domains API Get Link Shares",
    "_postman_id": "7f817d03-a6a9-4123-9481-5966709668b3",
    "description": "Returns metrics about a shares of a single link.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Shorten",
      "item": [
        {
          "id": "5be3730d-d055-4749-b3e8-1fc4f9c0c77a",
          "name": "Get_shorten_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/shorten?domain=%7B%7D&format=%7B%7D&longUrl=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given a long URL, returns a bitly short URL."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5900989c-24db-4a18-a632-0015cca90fa8"
            }
          ]
        }
      ]
    },
    {
      "name": "Expand",
      "item": [
        {
          "id": "040c4d75-a4c0-4d03-8fc5-defcc8293be6",
          "name": "Get_expand_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/expand?format=%7B%7D&hash=%7B%7D&shortUrl=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Given a bitly URL or hash (or multiple), returns the target (long) URL."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b9bca3e6-8262-4553-9ef3-00b1da7bb0ad"
            }
          ]
        }
      ]
    },
    {
      "name": "Link",
      "item": [
        {
          "id": "84af3a09-5073-41df-9c2b-6c59415b8ada",
          "name": "Get_lookup_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/link/lookup?format=%7B%7D&url=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This is used to query for a bitly link based on a long URL."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f2bfcc4b-ddd3-4bea-9d67-49d70f0fb532"
            }
          ]
        },
        {
          "id": "48234229-ec9d-4901-afef-d02bc1902fea",
          "name": "Get_link_clicks_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/link/clicks?format=%7B%7D&limit=%7B%7D&link=%7B%7D&rollup=%7B%7D&timezone=%7B%7D&unit=%7B%7D&units=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns entries from a user's link history in reverse chronological order."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ee9feba2-87ac-4361-a4d5-124e4e2633eb"
            }
          ]
        },
        {
          "id": "1aaf191c-8b29-495d-a947-a806c27cc442",
          "name": "Get_link_countries_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/link/countries?format=%7B%7D&limit=%7B%7D&link=%7B%7D&rollup=%7B%7D&timezone=%7B%7D&unit=%7B%7D&units=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns metrics about the countries referring click traffic to a single bitly link."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a5fa8394-2367-416a-8a24-495cd76deb4d"
            }
          ]
        },
        {
          "id": "f93a05e8-010d-4ed7-a24d-8553efad44c7",
          "name": "Get_link_referrers_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/link/referrers?format=%7B%7D&limit=%7B%7D&link=%7B%7D&rollup=%7B%7D&timezone=%7B%7D&unit=%7B%7D&units=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns metrics about the pages referring click traffic to a single bitly link."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b32a04d0-23d7-4c1b-bd5c-0822a025c374"
            }
          ]
        },
        {
          "id": "6a2fe177-0588-47d5-8815-eb1f13b267ef",
          "name": "Get_link_shares_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/link/shares?format=%7B%7D&limit=%7B%7D&link=%7B%7D&rollup=%7B%7D&timezone=%7B%7D&unit=%7B%7D&units=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns metrics about a shares of a single link."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1b0e6f14-a0e5-435d-9196-665ceac4c367"
            }
          ]
        }
      ]
    },
    {
      "name": "Info",
      "item": [
        {
          "id": "6874a9f2-d989-41da-b37b-eaa3db194548",
          "name": "Get_info_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/info?format=%7B%7D&hash=%7B%7D&shortUrl=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This is used to return the page title for a given bitly link."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8e2a33a3-9a40-4447-a896-6689e0794e36"
            }
          ]
        }
      ]
    },
    {
      "name": "User",
      "item": [
        {
          "id": "b192f527-9823-4719-b845-2532612e2250",
          "name": "Get_user_info_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/user/info?format=%7B%7D&login=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Return information about a user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f845b686-da86-4791-907b-e65285357aae"
            }
          ]
        },
        {
          "id": "cf3d656a-82dc-4eb9-bedd-e7160ba3cb19",
          "name": "Get_user_link_history_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/user/link_history?created_after=%7B%7D&created_before=%7B%7D&format=%7B%7D&limit=%7B%7D&user=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns entries from a user's link history in reverse chronological order."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "696e3d89-d0ea-4690-9028-fa218f4dc10a"
            }
          ]
        },
        {
          "id": "c1b1d8ea-679c-47e5-b4df-80ca0a896e24",
          "name": "Get_user_popular_links_",
          "request": {
            "url": "http://api-ssl.bitly.com/v3/user/popular_links?format=%7B%7D&limit=%7B%7D&rollup=%7B%7D&timezone=%7B%7D&unit=%7B%7D&units=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the authenticated user's most-clicked bitly links (ordered by number of clicks) in a given time period."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "feb2c8b0-08e8-406a-b40d-c09d56057243"
            }
          ]
        }
      ]
    }
  ]
}