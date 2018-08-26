{
  "info": {
    "name": "Ge.tt  REST API Shares Destroy",
    "_postman_id": "e6397334-fa27-4d7c-bcce-2b1d750f4170",
    "description": "Delete a share and all of its files.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Files",
      "item": [
        {
          "id": "0afad84b-64a8-41ed-b389-2473169959fa",
          "name": "post1FilesSharenameCreate",
          "request": {
            "url": {
              "protocol": "http",
              "host": "open.ge.tt",
              "path": [
                "1",
                "1/files/:sharename/create"
              ],
              "query": [
                {
                  "key": "accesstoken",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "sharename",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "To upload files to Ge.tt you must first create the file under a given share. You do that by posting the filename:"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f5387bb4-0010-4cc6-a69f-6209b4208fb1"
            }
          ]
        },
        {
          "id": "d52923df-0996-4491-9fef-38611751eb2e",
          "name": "get1FilesSharenameFile",
          "request": {
            "url": {
              "protocol": "http",
              "host": "open.ge.tt",
              "path": [
                "1",
                "1/files/:sharename/:fileid"
              ],
              "variable": [
                {
                  "id": "fileid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "sharename",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the state of a file. This returns the following data:"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f0c61675-f78f-4d96-abdf-f460c21a5060"
            }
          ]
        },
        {
          "id": "f937b044-0bcb-42d5-9bcb-c690adbf6547",
          "name": "get1FilesSharenameFileBlob",
          "request": {
            "url": {
              "protocol": "http",
              "host": "open.ge.tt",
              "path": [
                "1",
                "1/files/:sharename/:fileid/blob"
              ],
              "variable": [
                {
                  "id": "fileid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "sharename",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Will redirect to the binary content of the file"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "55f3343f-7e25-4611-b965-0cce6ef21279"
            }
          ]
        },
        {
          "id": "edd26301-1234-4d4f-9948-20ac429aa799",
          "name": "get1FilesSharenameFileBlobThumb",
          "request": {
            "url": {
              "protocol": "http",
              "host": "open.ge.tt",
              "path": [
                "1",
                "1/files/:sharename/:fileid/blob/thumb"
              ],
              "variable": [
                {
                  "id": "fileid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "sharename",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Will redirect to a thumbnail of the binary file. Currently only available for images."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0b036018-4001-4b82-901c-953d8ca6eacd"
            }
          ]
        },
        {
          "id": "ef935f93-fe21-486e-899c-7d1cb983e8ad",
          "name": "post1FilesSharenameFileDestroy",
          "request": {
            "url": {
              "protocol": "http",
              "host": "open.ge.tt",
              "path": [
                "1",
                "1/files/:sharename/:fileid/destroy"
              ],
              "query": [
                {
                  "key": "accesstoken",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "fileid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "sharename",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a file and the binary contents."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3f81525e-381d-4403-a721-497b7bc88aac"
            }
          ]
        },
        {
          "id": "6f231c6b-30e0-45e9-8d94-d4e847c64e34",
          "name": "get1FilesSharenameFileUpload",
          "request": {
            "url": {
              "protocol": "http",
              "host": "open.ge.tt",
              "path": [
                "1",
                "1/files/:sharename/:fileid/upload"
              ],
              "query": [
                {
                  "key": "accesstoken",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "fileid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "sharename",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get upload urls to the file. This returns a new PUT and POST url for you to upload the file to.nOBS You can also choose to use the put- or posturl that you were previously given to override the file."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "93d63dd0-fe78-4207-83d3-3652303db2c1"
            }
          ]
        }
      ]
    },
    {
      "name": "Shares",
      "item": [
        {
          "id": "66d1dc6d-700f-490f-ae68-f01ee95b2e34",
          "name": "get1Shares",
          "request": {
            "url": "http://open.ge.tt/1/1/shares?accesstoken=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns all your shares and the containing files:"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8d8b5c3c-75ce-480f-9d6f-fd657c3c557e"
            }
          ]
        },
        {
          "id": "76f3382b-4456-4d97-9f31-96079fea1e23",
          "name": "post1SharesCreate",
          "request": {
            "url": "http://open.ge.tt/1/1/shares/create?accesstoken=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new share. The request body is optional but can look like:"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2350c83e-255c-41e0-8e58-e7c2c08ced4d"
            }
          ]
        },
        {
          "id": "1abfa7b4-ed98-4600-8893-ec9e8f16dd39",
          "name": "get1SharesSharename",
          "request": {
            "url": {
              "protocol": "http",
              "host": "open.ge.tt",
              "path": [
                "1",
                "1/shares/:sharename"
              ],
              "variable": [
                {
                  "id": "sharename",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists a share."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6448be85-e33e-4027-bccc-9af72d90f6fe"
            }
          ]
        },
        {
          "id": "6d1e437a-fa64-4810-9bab-f28e07521260",
          "name": "post1SharesSharenameDestroy",
          "request": {
            "url": {
              "protocol": "http",
              "host": "open.ge.tt",
              "path": [
                "1",
                "1/shares/:sharename/destroy"
              ],
              "query": [
                {
                  "key": "accesstoken",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "sharename",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a share and all of its files."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4a909981-d94c-4f98-82f6-d19ab9cf6df5"
            }
          ]
        }
      ]
    }
  ]
}