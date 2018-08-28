{
  "info": {
    "name": "AWS Storage Gateway Service API List File Shares",
    "_postman_id": "23733d59-c6f2-44c8-9ceb-9b4fcd0734e4",
    "description": "Gets a list of the file shares for a specific file gateway, or the list of file shares that belong to the calling user account.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Gateway",
      "item": [
        {
          "id": "c8a54bae-dd2a-4f42-a2fe-4355815f31b2",
          "name": "activateGateway",
          "request": {
            "url": "http://example.com/api/?Action=ActivateGateway?ActivationKey=ActivationKey&GatewayName=GatewayName&GatewayRegion=GatewayRegion&GatewayTimezone=GatewayTimezone&GatewayType=GatewayType&MediumChangerType=MediumChangerType&TapeDriveType=TapeDriveType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Activates the gateway you previously deployed on your host."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b8d14fed-cbdc-45ca-b086-97ae56ce138e"
            }
          ]
        },
        {
          "id": "76242984-5d36-4319-a511-38c4205323c3",
          "name": "deleteGateway",
          "request": {
            "url": "http://example.com/api/?Action=DeleteGateway?GatewayARN=GatewayARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a gateway."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "109db46b-f23b-4191-80e9-4b82c8cc62a0"
            }
          ]
        },
        {
          "id": "dea9cb52-cf21-42b9-a29b-bd2eb830379b",
          "name": "describeGatewayInformation",
          "request": {
            "url": "http://example.com/api/?Action=DescribeGatewayInformation?GatewayARN=GatewayARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns metadata about a gateway such as its name, network interfaces, configured\n         time zone, and the state (whether the gateway is running or not)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4acedddf-3393-4840-baa5-f700e1939e31"
            }
          ]
        },
        {
          "id": "e53505a2-c04a-4c81-b895-d683c10009c2",
          "name": "disableGateway",
          "request": {
            "url": "http://example.com/api/?Action=DisableGateway?GatewayARN=GatewayARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Disables a gateway when the gateway is no longer functioning."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eba1647b-64eb-4c20-8434-69a3c4a6a616"
            }
          ]
        }
      ]
    },
    {
      "name": "Cache",
      "item": [
        {
          "id": "19e03335-b4b8-450c-b7fa-4d9809fbee8c",
          "name": "addCache",
          "request": {
            "url": "http://example.com/api/?Action=AddCache?DiskIds=DiskIds&GatewayARN=GatewayARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Configures one or more gateway local disks as cache for a cached-volume gateway."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "af12e966-189f-4efa-bb58-c28b2ce52d7a"
            }
          ]
        },
        {
          "id": "d4a3a10e-e485-480f-81da-d767736cd066",
          "name": "describeCache",
          "request": {
            "url": "http://example.com/api/?Action=DescribeCache?GatewayARN=GatewayARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about the cache of a gateway."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "66bcdbfd-5f47-4b15-bbcf-92ebd1796003"
            }
          ]
        }
      ]
    },
    {
      "name": "Tags",
      "item": [
        {
          "id": "e47ef262-b4ff-414a-b746-fcb184c2bffe",
          "name": "addTagsToResource",
          "request": {
            "url": "http://example.com/api/?Action=AddTagsToResource?ResourceARN=ResourceARN&Tags=Tags",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds one or more tags to the specified resource."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0b2bd75e-a9ed-4b1d-b627-d5be3ed1375f"
            }
          ]
        }
      ]
    },
    {
      "name": "Upload Buffer",
      "item": [
        {
          "id": "9efa1d9e-156d-4750-b8ae-6ef39599549c",
          "name": "addUploadBuffer",
          "request": {
            "url": "http://example.com/api/?Action=AddUploadBuffer?DiskIds=DiskIds&GatewayARN=GatewayARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Configures one or more gateway local disks as upload buffer for a specified gateway."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "65fd2417-f665-4fd1-be9d-abcf3bf06219"
            }
          ]
        },
        {
          "id": "e837f75d-c61b-493d-869f-5211c2ee9814",
          "name": "describeUploadBuffer",
          "request": {
            "url": "http://example.com/api/?Action=DescribeUploadBuffer?GatewayARN=GatewayARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about the upload buffer of a gateway."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "44b9c9bb-e70b-4901-920d-a94ce1b7a3bd"
            }
          ]
        }
      ]
    },
    {
      "name": "Working Storage",
      "item": [
        {
          "id": "d68a071f-e19a-4289-95ad-da3c5eda96b7",
          "name": "addWorkingStorage",
          "request": {
            "url": "http://example.com/api/?Action=AddWorkingStorage?DiskIds=DiskIds&GatewayARN=GatewayARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Configures one or more gateway local disks as working storage for a gateway."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5331c452-3d96-48e7-b07c-864ab85e982a"
            }
          ]
        },
        {
          "id": "8903d858-dc8c-429b-8d86-9a15ffb160a9",
          "name": "describeWorkingStorage",
          "request": {
            "url": "http://example.com/api/?Action=DescribeWorkingStorage?GatewayARN=GatewayARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about the working storage of a gateway."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9defb626-3328-42ee-bcc5-33207fdb0cfe"
            }
          ]
        }
      ]
    },
    {
      "name": "Archival",
      "item": [
        {
          "id": "6e271480-e213-40e4-9378-327244a56322",
          "name": "cancelArchival",
          "request": {
            "url": "http://example.com/api/?Action=CancelArchival?GatewayARN=GatewayARN&TapeARN=TapeARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Cancels archiving of a virtual tape to the virtual tape shelf (VTS) after the\n         archiving process is initiated."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8bdfd3ae-a4b0-4ea5-a961-34a19f8ad897"
            }
          ]
        }
      ]
    },
    {
      "name": "Retrieval",
      "item": [
        {
          "id": "c39c31db-f5e4-4434-a4d1-d1b95bf84b0d",
          "name": "cancelRetrieval",
          "request": {
            "url": "http://example.com/api/?Action=CancelRetrieval?GatewayARN=GatewayARN&TapeARN=TapeARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Cancels retrieval of a virtual tape from the virtual tape shelf (VTS) to a gateway\n         after the retrieval process is initiated."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "32bb84ea-7307-4e9d-9df6-d703162c4b54"
            }
          ]
        }
      ]
    },
    {
      "name": "Cached SCSI Volume",
      "item": [
        {
          "id": "40952616-bf54-46a9-a77c-06d13e087933",
          "name": "createCachediSCSIVolume",
          "request": {
            "url": "http://example.com/api/?Action=CreateCachediSCSIVolume?ClientToken=ClientToken&GatewayARN=GatewayARN&NetworkInterfaceId=NetworkInterfaceId&SnapshotId=SnapshotId&SourceVolumeARN=SourceVolumeARN&TargetName=TargetName&VolumeSizeInBytes=VolumeSizeInBytes",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a cached volume on a specified cached gateway."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "29afe5a8-f783-4305-802a-6ddf889286a6"
            }
          ]
        }
      ]
    },
    {
      "name": "NFS File Share",
      "item": [
        {
          "id": "ad5474bb-2ac7-45cf-bbc2-80c44df8150a",
          "name": "createNFSFileShare",
          "request": {
            "url": "http://example.com/api/?Action=CreateNFSFileShare?ClientToken=ClientToken&DefaultStorageClass=DefaultStorageClass&GatewayARN=GatewayARN&KMSEncrypted=KMSEncrypted&KMSKey=KMSKey&LocationARN=LocationARN&NFSFileShareDefaults=NFSFileShareDefaults&Role=Role",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a file share on an existing file gateway."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d34f030f-390b-4dd7-b399-060297096eae"
            }
          ]
        }
      ]
    },
    {
      "name": "Snapshots",
      "item": [
        {
          "id": "96ba0ca5-f024-4b7e-95e6-8fa5a8abb5e9",
          "name": "createSnapshot",
          "request": {
            "url": "http://example.com/api/?Action=CreateSnapshot?SnapshotDescription=SnapshotDescription&VolumeARN=VolumeARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Initiates a snapshot of a volume."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2b837cec-9cd4-466d-8978-34dfbed32aa2"
            }
          ]
        },
        {
          "id": "b29809bc-0fb6-4f62-bf56-4ab8939452fd",
          "name": "createSnapshotFromVolumeRecoveryPoint",
          "request": {
            "url": "http://example.com/api/?Action=CreateSnapshotFromVolumeRecoveryPoint?SnapshotDescription=SnapshotDescription&VolumeARN=VolumeARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Initiates a snapshot of a gateway from a volume recovery point."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6d32efed-0972-4ea9-9dd6-329cfe84942e"
            }
          ]
        },
        {
          "id": "ab497b41-84a3-4872-b4a1-956b684c8e2e",
          "name": "deleteSnapshotSchedule",
          "request": {
            "url": "http://example.com/api/?Action=DeleteSnapshotSchedule?VolumeARN=VolumeARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a snapshot of a volume."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7131d580-fbad-4454-b1be-64fe9e09143c"
            }
          ]
        },
        {
          "id": "b8d1acdc-cf27-4ee6-8c38-6cd05ed5af2d",
          "name": "describeSnapshotSchedule",
          "request": {
            "url": "http://example.com/api/?Action=DescribeSnapshotSchedule?VolumeARN=VolumeARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Describes the snapshot schedule for the specified gateway volume."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "db1e4e24-0cce-49d4-a1ec-2cfd513bdd66"
            }
          ]
        }
      ]
    },
    {
      "name": "Stored SCSI Volume",
      "item": [
        {
          "id": "ea633665-3fb9-4c19-80df-1e371fd03679",
          "name": "createStorediSCSIVolume",
          "request": {
            "url": "http://example.com/api/?Action=CreateStorediSCSIVolume?DiskId=DiskId&GatewayARN=GatewayARN&NetworkInterfaceId=NetworkInterfaceId&PreserveExistingData=PreserveExistingData&SnapshotId=SnapshotId&TargetName=TargetName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a volume on a specified gateway."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f3e7ff98-bd73-479d-b503-9e939536ab9b"
            }
          ]
        }
      ]
    },
    {
      "name": "Tapes",
      "item": [
        {
          "id": "204901d4-e41d-4e04-afb4-4c6dd3b2968e",
          "name": "createTapes",
          "request": {
            "url": "http://example.com/api/?Action=CreateTapes?ClientToken=ClientToken&GatewayARN=GatewayARN&NumTapesToCreate=NumTapesToCreate&TapeBarcodePrefix=TapeBarcodePrefix&TapeSizeInBytes=TapeSizeInBytes",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates one or more virtual tapes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6b1e5382-b75b-4bc6-8b1a-7bbf82e34eb5"
            }
          ]
        },
        {
          "id": "a3e49490-ef75-4f80-acb4-a11304ad1a21",
          "name": "deleteTape",
          "request": {
            "url": "http://example.com/api/?Action=DeleteTape?GatewayARN=GatewayARN&TapeARN=TapeARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified virtual tape."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b315e0e0-1171-47c9-84d7-a899763f5602"
            }
          ]
        },
        {
          "id": "1f49b42d-fcbe-4a0a-92b1-1ee7da0d3378",
          "name": "deleteTapeArchive",
          "request": {
            "url": "http://example.com/api/?Action=DeleteTapeArchive?TapeARN=TapeARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified virtual tape from the virtual tape shelf (VTS)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "36410d75-252c-41be-ac7c-2fbea65adce1"
            }
          ]
        },
        {
          "id": "e6f083e6-f580-4604-9355-daef222b5c1e",
          "name": "describeTapes",
          "request": {
            "url": "http://example.com/api/?Action=DescribeTapes?GatewayARN=GatewayARN&Limit=Limit&Marker=Marker&TapeARNs=TapeARNs",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a description of the specified Amazon Resource Name (ARN) of virtual tapes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "05cbcdd8-a98c-4634-b869-7e1e7c12e947"
            }
          ]
        }
      ]
    },
    {
      "name": "Tape With Barcode",
      "item": [
        {
          "id": "df6ea67b-c5f3-4bfb-9b9c-5177852c70fe",
          "name": "createTapeWithBarcode",
          "request": {
            "url": "http://example.com/api/?Action=CreateTapeWithBarcode?GatewayARN=GatewayARN&TapeBarcode=TapeBarcode&TapeSizeInBytes=TapeSizeInBytes",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a virtual tape by using your own barcode."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "72f66d50-b08e-4010-a5bb-1231b38ec28a"
            }
          ]
        }
      ]
    },
    {
      "name": "Bandwidth Rate Limit",
      "item": [
        {
          "id": "10add139-17c1-41c4-aa45-0cb3f652abf3",
          "name": "deleteBandwidthRateLimit",
          "request": {
            "url": "http://example.com/api/?Action=DeleteBandwidthRateLimit?BandwidthType=BandwidthType&GatewayARN=GatewayARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the bandwidth rate limits of a gateway."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eeac2748-cef1-4093-9cbc-880606eb958e"
            }
          ]
        },
        {
          "id": "7c47bbca-0fd7-4097-8be3-5547ee2be2db",
          "name": "describeBandwidthRateLimit",
          "request": {
            "url": "http://example.com/api/?Action=DescribeBandwidthRateLimit?GatewayARN=GatewayARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the bandwidth rate limits of a gateway."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e4e4c2c4-630a-44f0-bf07-cf6a733718bc"
            }
          ]
        }
      ]
    },
    {
      "name": "Chap Credentials",
      "item": [
        {
          "id": "8ed800a6-a4b7-441a-a681-e4df77c33f0c",
          "name": "deleteChapCredentials",
          "request": {
            "url": "http://example.com/api/?Action=DeleteChapCredentials?InitiatorName=InitiatorName&TargetARN=TargetARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes Challenge-Handshake Authentication Protocol (CHAP) credentials for a\n         specified iSCSI target and initiator pair."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5104d5b6-bb4e-4f51-ae2c-1965a246ca82"
            }
          ]
        },
        {
          "id": "594961ec-b7f0-452e-9066-c9e45d4bdab2",
          "name": "describeChapCredentials",
          "request": {
            "url": "http://example.com/api/?Action=DescribeChapCredentials?TargetARN=TargetARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns an array of Challenge-Handshake Authentication Protocol (CHAP) credentials\n         information for a specified iSCSI target, one for each target-initiator pair."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "99ccd0f2-cdff-447d-9e6e-3de6a5f5eb06"
            }
          ]
        }
      ]
    },
    {
      "name": "File Share",
      "item": [
        {
          "id": "660670d2-ad8e-4229-8604-41608bf0f746",
          "name": "deleteFileShare",
          "request": {
            "url": "http://example.com/api/?Action=DeleteFileShare?FileShareARN=FileShareARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a file share from a file gateway."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "051e3397-4485-474a-9ceb-2a91be642b22"
            }
          ]
        }
      ]
    },
    {
      "name": "Volumes",
      "item": [
        {
          "id": "bac912bc-a315-4671-b71f-043afab23a7a",
          "name": "deleteVolume",
          "request": {
            "url": "http://example.com/api/?Action=DeleteVolume?VolumeARN=VolumeARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified gateway volume that you previously created using the."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "77112443-9f8c-4a7a-a3cb-52b0d62b3531"
            }
          ]
        }
      ]
    },
    {
      "name": "Cached SCSI Volumes",
      "item": [
        {
          "id": "57a55504-3536-4f25-b0fd-f302b518384f",
          "name": "describeCachediSCSIVolumes",
          "request": {
            "url": "http://example.com/api/?Action=DescribeCachediSCSIVolumes?VolumeARNs=VolumeARNs",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a description of the gateway volumes specified in the request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "00b05866-659b-4f40-a3ca-503788ccf477"
            }
          ]
        }
      ]
    },
    {
      "name": "Maintenance",
      "item": [
        {
          "id": "7b4d95ee-eb0e-4065-bf8a-8de388039a01",
          "name": "describeMaintenanceStartTime",
          "request": {
            "url": "http://example.com/api/?Action=DescribeMaintenanceStartTime?GatewayARN=GatewayARN",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns your gateway's weekly maintenance start time including the day and time of\n         the week."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "170444f2-d334-4730-b85f-11b5cc7b4bfb"
            }
          ]
        }
      ]
    },
    {
      "name": "NFS File Shares",
      "item": [
        {
          "id": "19951601-b651-4d30-9159-4fa9c2f9d9bc",
          "name": "describeNFSFileShares",
          "request": {
            "url": "http://example.com/api/?Action=DescribeNFSFileShares?FileShareARNList=FileShareARNList",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a description for one or more file shares from a file gateway."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "77606cb2-7e20-465e-9936-6610f49f2af8"
            }
          ]
        }
      ]
    },
    {
      "name": "Stored SCSI Volumes",
      "item": [
        {
          "id": "483ff5a3-b7a5-4b1c-8be3-81606bab98e2",
          "name": "describeStorediSCSIVolumes",
          "request": {
            "url": "http://example.com/api/?Action=DescribeStorediSCSIVolumes?VolumeARNs=VolumeARNs",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the description of the gateway volumes specified in the request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9aa4a3fe-79c2-4ee3-b578-662e66a35a72"
            }
          ]
        }
      ]
    },
    {
      "name": "Tape Archives",
      "item": [
        {
          "id": "f1ecf423-f079-461f-820d-1bd19bf77f6a",
          "name": "describeTapeArchives",
          "request": {
            "url": "http://example.com/api/?Action=DescribeTapeArchives?Limit=Limit&Marker=Marker&TapeARNs=TapeARNs",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a description of specified virtual tapes in the virtual tape shelf\n         (VTS)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e1325ad0-3e59-4237-be5c-896dfa0f3f91"
            }
          ]
        }
      ]
    },
    {
      "name": "Tape Recovery Points",
      "item": [
        {
          "id": "0c4b883e-779e-4f61-9839-c1b48f8fded9",
          "name": "describeTapeRecoveryPoints",
          "request": {
            "url": "http://example.com/api/?Action=DescribeTapeRecoveryPoints?GatewayARN=GatewayARN&Limit=Limit&Marker=Marker",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of virtual tape recovery points that are available for the specified\n         gateway-VTL."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "698fa046-a2b4-4838-8aa0-cea7bbfcfbb7"
            }
          ]
        }
      ]
    },
    {
      "name": "VTL Devices",
      "item": [
        {
          "id": "a490ca52-3008-46e3-bf77-b96fec0a0842",
          "name": "describeVTLDevices",
          "request": {
            "url": "http://example.com/api/?Action=DescribeVTLDevices?GatewayARN=GatewayARN&Limit=Limit&Marker=Marker&VTLDeviceARNs=VTLDeviceARNs",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a description of virtual tape library (VTL) devices for the specified\n         gateway."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0a654cec-8ffb-4b12-a1c1-298f9f15ccc6"
            }
          ]
        }
      ]
    },
    {
      "name": "File Shares",
      "item": [
        {
          "id": "192f806c-6f69-49c2-9baa-44bf720afe88",
          "name": "listFileShares",
          "request": {
            "url": "http://example.com/api/?Action=ListFileShares?GatewayARN=GatewayARN&Limit=Limit&Marker=Marker",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a list of the file shares for a specific file gateway, or the list of file shares that belong to the calling user account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f7d21540-f464-4b40-aaf4-924de7a28a15"
            }
          ]
        }
      ]
    }
  ]
}