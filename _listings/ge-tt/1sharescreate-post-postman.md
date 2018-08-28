{
  "info": {
    "name": "Ge.tt  REST API Shares Create",
    "_postman_id": "5388b81f-0394-4ea8-8b70-05ed20676e6b",
    "description": "Creates a new share. The request body is optional but can look like:",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Files",
      "item": [
        {
          "id": "0049308e-8b7d-41bf-8f27-6227ea68ab91",
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
              "id": "460735e3-4a88-43f3-b6c4-44d2127828c9"
            }
          ]
        },
        {
          "id": "d0fb2e99-aaa0-4ada-839e-8a9e0f37a506",
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
              "id": "af4b9f75-d9d5-4268-9955-df9f1e2c2c78"
            }
          ]
        },
        {
          "id": "d84d28ac-5718-4816-b567-cb3106bde8ea",
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
              "id": "039a1dd7-a041-4829-ba47-cad8ea586494"
            }
          ]
        },
        {
          "id": "dd443511-4a5c-41b7-8c7e-bd20b9031053",
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
              "id": "0e2c5a89-da55-4e2e-bb4a-fd3d3cd522fe"
            }
          ]
        },
        {
          "id": "39e290b5-32e4-4b34-b64d-d8c44c0a2aeb",
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
              "id": "22c00217-b93b-437b-9722-ed06a612b33e"
            }
          ]
        },
        {
          "id": "6619f2dc-eb5e-4f89-98f2-8337921d35e4",
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
              "id": "aac3739a-004e-4e8f-83af-0dea11a1e2f9"
            }
          ]
        }
      ]
    },
    {
      "name": "Shares",
      "item": [
        {
          "id": "da2e95c2-a616-4f71-b948-c9da0ef6284c",
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
              "id": "0c324651-8dc2-41bb-8ffa-1f2fba6dbbd6"
            }
          ]
        },
        {
          "id": "219443d7-a4f3-461d-8b2c-368d45a9736f",
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
              "id": "87257e30-1a2c-491b-9d39-bfd76977ccd0"
            }
          ]
        }
      ]
    }
  ]
}