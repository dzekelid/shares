{
  "info": {
    "name": "Ge.tt  REST API Shares",
    "_postman_id": "34be4b4f-aff2-4849-84c9-fdf4c40def5f",
    "description": "Lists a share.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Files",
      "item": [
        {
          "id": "ae58d80d-b02d-41c1-b6f6-c3000b8d72bd",
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
              "id": "461b16fb-4c07-48ea-98dc-edfb8d8367e0"
            }
          ]
        },
        {
          "id": "e4ccb565-ec5c-4ef5-b6b1-2d7a99bb4117",
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
              "id": "cf21aef9-32f2-46c9-9953-1e4b4bb6a6cf"
            }
          ]
        },
        {
          "id": "f51a677d-8076-4e94-97ce-9fd88fcf1776",
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
              "id": "34dd9642-4c1a-425b-b5a3-2ea5f000d09f"
            }
          ]
        },
        {
          "id": "46e911ad-d698-4508-a299-97db51442246",
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
              "id": "aa7050e3-b287-41d1-87c8-9d5a92479bbb"
            }
          ]
        },
        {
          "id": "c2d3faf1-66b7-4949-8b17-1cd34e4db3c3",
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
              "id": "b6620788-3677-495a-b61a-33c1e7688a37"
            }
          ]
        },
        {
          "id": "c192bbf6-ce65-4f0e-b4e0-0fcba877b6d5",
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
              "id": "8cf10cf3-a323-49fe-a2e2-b2f2d03ee9c5"
            }
          ]
        }
      ]
    },
    {
      "name": "Shares",
      "item": [
        {
          "id": "5dd42a7d-f094-4f1f-902e-e7b2b24463e9",
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
              "id": "f398214c-873b-441f-b3e0-4533bcb36007"
            }
          ]
        },
        {
          "id": "81d8b2f3-ae9d-4c94-9d22-29fa1e7dffaf",
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
              "id": "e8a0586a-556c-4818-99b3-14eedc703dee"
            }
          ]
        },
        {
          "id": "4effd143-3705-42df-af13-95a3ad31cfc4",
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
              "id": "0f3abde6-0b41-4f2c-9ae8-f06f4481f2f4"
            }
          ]
        }
      ]
    }
  ]
}