{
  "info": {
    "name": "AWS Directory Service API Update Conditional Forwarder",
    "_postman_id": "9a2bcb3c-9260-4156-995a-d19dd10b5178",
    "description": "Updates a conditional forwarder that has been set up for your AWS directory.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "IP Address Routes",
      "item": [
        {
          "id": "b1eb35a0-b72e-43d3-89a9-42302c067731",
          "name": "addIpRoutes",
          "request": {
            "url": "http://example.com/api/?Action=AddIpRoutes?DirectoryId=DirectoryId&IpRoutes=IpRoutes&UpdateSecurityGroupForDirectoryControllers=UpdateSecurityGroupForDirectoryControllers",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "If the DNS server for your on-premises domain uses a publicly addressable IP address, you must add a CIDR address block to correctly route traffic to and from your Microsoft AD on Amazon Web Services."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "900d96ab-ffa5-4d1d-85d9-ec1fa91d5569"
            }
          ]
        },
        {
          "id": "a22547d2-38a4-4d9b-b81c-312f225083bf",
          "name": "listIpRoutes",
          "request": {
            "url": "http://example.com/api/?Action=ListIpRoutes?DirectoryId=DirectoryId&Limit=Limit&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the address blocks that you have added to a directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "967c0d73-2ffb-44ae-8566-1ab3d84cfede"
            }
          ]
        },
        {
          "id": "65372c56-04de-4425-ad5a-5e0eb45809f4",
          "name": "removeIpRoutes",
          "request": {
            "url": "http://example.com/api/?Action=RemoveIpRoutes?CidrIps=CidrIps&DirectoryId=DirectoryId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes IP address blocks from a directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4a5b637f-e519-4e82-bab6-ca9f55dc69db"
            }
          ]
        }
      ]
    },
    {
      "name": "Resource Tags",
      "item": [
        {
          "id": "166c83c1-ae5e-4e55-9d36-9043f4497fbe",
          "name": "addTagsToResource",
          "request": {
            "url": "http://example.com/api/?Action=AddTagsToResource?ResourceId=ResourceId&Tags=Tags",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds or overwrites one or more tags for the specified directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ffbf4eed-85a5-4a26-ab31-915bfbb76285"
            }
          ]
        },
        {
          "id": "15023eee-d2ab-43b5-b96c-19c7bf12ec62",
          "name": "listTagsForResource",
          "request": {
            "url": "http://example.com/api/?Action=ListTagsForResource?Limit=Limit&NextToken=NextToken&ResourceId=ResourceId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all tags on a directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6780f103-32ab-48e1-9869-11944685811a"
            }
          ]
        },
        {
          "id": "1a24d81a-aaf5-4ac3-aa99-16bb11d113c7",
          "name": "removeTagsFromResource",
          "request": {
            "url": "http://example.com/api/?Action=RemoveTagsFromResource?ResourceId=ResourceId&TagKeys=TagKeys",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes tags from a directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c25c4eb6-e393-46fc-8375-37cafe6c9a61"
            }
          ]
        }
      ]
    },
    {
      "name": "Schemas",
      "item": [
        {
          "id": "a28dc1c0-f7ba-4e3f-a647-d1a82788b13d",
          "name": "cancelSchemaExtension",
          "request": {
            "url": "http://example.com/api/?Action=CancelSchemaExtension?DirectoryId=DirectoryId&SchemaExtensionId=SchemaExtensionId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Cancels an in-progress schema extension to a Microsoft AD directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9e73680e-42a7-4c22-9909-f16c0e7e5d48"
            }
          ]
        }
      ]
    },
    {
      "name": "Directories",
      "item": [
        {
          "id": "607fd4b6-7a47-4151-b4e4-4aa43523176d",
          "name": "connectDirectory",
          "request": {
            "url": "http://example.com/api/?Action=ConnectDirectory?ConnectSettings=ConnectSettings&Description=Description&Name=Name&Password=Password&ShortName=ShortName&Size=Size",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an AD Connector to connect to an on-premises directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8d9b858e-4a18-4eb4-b1dc-9d88a3ed39c2"
            }
          ]
        },
        {
          "id": "b65f572e-b65c-4cc5-b82a-e8c537ec1a8f",
          "name": "createDirectory",
          "request": {
            "url": "http://example.com/api/?Action=CreateDirectory?Description=Description&Name=Name&Password=Password&ShortName=ShortName&Size=Size&VpcSettings=VpcSettings",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a Simple AD directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a65fac2b-18be-4e8a-a614-735b0f003d91"
            }
          ]
        },
        {
          "id": "b9dc9387-0ab4-4676-b517-594298870040",
          "name": "deleteDirectory",
          "request": {
            "url": "http://example.com/api/?Action=DeleteDirectory?DirectoryId=DirectoryId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an AWS Directory Service directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b15b6857-8d07-4cdd-aa2f-3cd7fd442b94"
            }
          ]
        },
        {
          "id": "da1ffdb4-281e-4576-b940-0b21922b3039",
          "name": "describeDirectories",
          "request": {
            "url": "http://example.com/api/?Action=DescribeDirectories?DirectoryIds=DirectoryIds&Limit=Limit&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Obtains information about the directories that belong to this account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "93ec80f9-bc2c-495e-88dc-6c7c20de9062"
            }
          ]
        },
        {
          "id": "db1129d3-d6bb-4ff5-aaf9-0c4133da42cd",
          "name": "getDirectoryLimits",
          "request": {
            "url": "http://example.com/api/?Action=GetDirectoryLimits?DirectoryLimits=DirectoryLimits",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Obtains directory limit information for the current region."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ce1f895b-884a-412a-8a4a-5d949e44117f"
            }
          ]
        }
      ]
    },
    {
      "name": "Alias",
      "item": [
        {
          "id": "68a3841d-7a7a-415f-ad56-43034842466b",
          "name": "createAlias",
          "request": {
            "url": "http://example.com/api/?Action=CreateAlias?Alias=Alias&DirectoryId=DirectoryId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates an alias for a directory and assigns the alias to the directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "34c47879-fc46-4289-81ef-812867f57135"
            }
          ]
        }
      ]
    },
    {
      "name": "Computer",
      "item": [
        {
          "id": "bed54513-6031-4ed9-af52-975af5f719fd",
          "name": "createComputer",
          "request": {
            "url": "http://example.com/api/?Action=CreateComputer?ComputerAttributes=ComputerAttributes&ComputerName=ComputerName&DirectoryId=DirectoryId&OrganizationalUnitDistinguishedName=OrganizationalUnitDistinguishedName&Password=Password",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a computer account in the specified directory, and joins the computer to the directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f9c5b47a-212e-4e75-953e-881b090579b2"
            }
          ]
        }
      ]
    },
    {
      "name": "Conditional Forwarder",
      "item": [
        {
          "id": "bd8fc333-b29b-4dec-930b-a9660418561c",
          "name": "createConditionalForwarder",
          "request": {
            "url": "http://example.com/api/?Action=CreateConditionalForwarder?DirectoryId=DirectoryId&DnsIpAddrs=DnsIpAddrs&RemoteDomainName=RemoteDomainName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a conditional forwarder associated with your AWS directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3e4bd4e6-7b62-4fed-b425-e0595dbc3841"
            }
          ]
        },
        {
          "id": "bf3b9fd3-fa13-44a8-933d-b7e0aa53ef7f",
          "name": "deleteConditionalForwarder",
          "request": {
            "url": "http://example.com/api/?Action=DeleteConditionalForwarder?DirectoryId=DirectoryId&RemoteDomainName=RemoteDomainName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a conditional forwarder that has been set up for your AWS directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "123bdf1d-0636-4cc4-b6e1-e2316cd8a29b"
            }
          ]
        },
        {
          "id": "0357155b-e825-4b99-86c7-98999cf3de9f",
          "name": "describeConditionalForwarders",
          "request": {
            "url": "http://example.com/api/?Action=DescribeConditionalForwarders?DirectoryId=DirectoryId&RemoteDomainNames=RemoteDomainNames",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Obtains information about the conditional forwarders for this account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "19a50985-ddb8-4ec4-af1f-e8e072dbe843"
            }
          ]
        },
        {
          "id": "ac75cf27-ebf7-439e-b160-198d0df60222",
          "name": "updateConditionalForwarder",
          "request": {
            "url": "http://example.com/api/?Action=UpdateConditionalForwarder?DirectoryId=DirectoryId&DnsIpAddrs=DnsIpAddrs&RemoteDomainName=RemoteDomainName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Updates a conditional forwarder that has been set up for your AWS directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ee8e0389-8a1c-4879-8fbb-c89228442fcf"
            }
          ]
        }
      ]
    },
    {
      "name": "Microsoft AD",
      "item": [
        {
          "id": "c3fb98f7-0c9a-4fca-9158-22697671b51e",
          "name": "createMicrosoftAD",
          "request": {
            "url": "http://example.com/api/?Action=CreateMicrosoftAD?Description=Description&Name=Name&Password=Password&ShortName=ShortName&VpcSettings=VpcSettings",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a Microsoft AD in the AWS cloud."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9ab7f5ae-c16c-44eb-b0bd-5c79e4f85571"
            }
          ]
        }
      ]
    },
    {
      "name": "Snapshot",
      "item": [
        {
          "id": "8763183a-5100-4041-a05c-086e15662722",
          "name": "createSnapshot",
          "request": {
            "url": "http://example.com/api/?Action=CreateSnapshot?DirectoryId=DirectoryId&Name=Name",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a snapshot of a Simple AD or Microsoft AD directory in the AWS cloud."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "581a2d60-f1af-4027-a00c-07d4d04cef11"
            }
          ]
        }
      ]
    },
    {
      "name": "Trust",
      "item": [
        {
          "id": "2d5524a3-19db-4d06-89dd-64b710ea0731",
          "name": "createTrust",
          "request": {
            "url": "http://example.com/api/?Action=CreateTrust?ConditionalForwarderIpAddrs=ConditionalForwarderIpAddrs&DirectoryId=DirectoryId&RemoteDomainName=RemoteDomainName&TrustDirection=TrustDirection&TrustPassword=TrustPassword&TrustType=TrustType",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "AWS Directory Service for Microsoft Active Directory allows you to configure trust relationships."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "32e5f049-4c1f-4a01-b095-d2773d7554e4"
            }
          ]
        },
        {
          "id": "9bc79f1b-4217-429b-9ec0-57e83b4e682c",
          "name": "deleteTrust",
          "request": {
            "url": "http://example.com/api/?Action=DeleteTrust?DeleteAssociatedConditionalForwarder=DeleteAssociatedConditionalForwarder&TrustId=TrustId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an existing trust relationship between your Microsoft AD in the AWS cloud and an external domain."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e5f70fbe-c86f-41d2-b2f5-fcb74dc45196"
            }
          ]
        },
        {
          "id": "f39a2b39-df08-48bb-9b73-a2de21208b54",
          "name": "describeTrusts",
          "request": {
            "url": "http://example.com/api/?Action=DescribeTrusts?DirectoryId=DirectoryId&Limit=Limit&NextToken=NextToken&TrustIds=TrustIds",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Obtains information about the trust relationships for this account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d0faa1b3-4d66-45c4-b57c-7d5679120066"
            }
          ]
        }
      ]
    },
    {
      "name": "Snapshots",
      "item": [
        {
          "id": "d5bf4b2c-5c80-4d93-b28a-0eb327be76de",
          "name": "deleteSnapshot",
          "request": {
            "url": "http://example.com/api/?Action=DeleteSnapshot?SnapshotId=SnapshotId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a directory snapshot."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "92a57344-ae26-4051-900f-596771cecc73"
            }
          ]
        },
        {
          "id": "2e2f7b90-8dfc-4d90-89d9-0f9af5ad2ae2",
          "name": "describeSnapshots",
          "request": {
            "url": "http://example.com/api/?Action=DescribeSnapshots?DirectoryId=DirectoryId&Limit=Limit&NextToken=NextToken&SnapshotIds=SnapshotIds",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Obtains information about the directory snapshots that belong to this account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c4f8ce45-a3cf-499d-8094-9688f832e3d6"
            }
          ]
        },
        {
          "id": "3546644c-5c4c-4eeb-9dd6-7124cebea301",
          "name": "getSnapshotLimits",
          "request": {
            "url": "http://example.com/api/?Action=GetSnapshotLimits?DirectoryId=DirectoryId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Obtains the manual snapshot limits for a directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "611fea60-466b-422a-9655-a83992911185"
            }
          ]
        },
        {
          "id": "6a96352d-0a78-4a10-9c16-8e398705a80c",
          "name": "restoreFromSnapshot",
          "request": {
            "url": "http://example.com/api/?Action=RestoreFromSnapshot?SnapshotId=SnapshotId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Restores a directory using an existing directory snapshot."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "81fe478f-7df1-4bf5-9fbd-e55257134af3"
            }
          ]
        }
      ]
    },
    {
      "name": "Events",
      "item": [
        {
          "id": "4c002a89-b275-4941-b212-73c86e46108d",
          "name": "deregisterEventTopic",
          "request": {
            "url": "http://example.com/api/?Action=DeregisterEventTopic?DirectoryId=DirectoryId&TopicName=TopicName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Removes the specified directory as a publisher to the specified SNS topic."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "58f798df-157f-4d25-a3e3-0abacc0024af"
            }
          ]
        },
        {
          "id": "9fac9096-cbd9-4fa4-9cdb-495209c7ba4e",
          "name": "describeEventTopics",
          "request": {
            "url": "http://example.com/api/?Action=DescribeEventTopics?DirectoryId=DirectoryId&TopicNames=TopicNames",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Obtains information about which SNS topics receive status messages from the specified directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7342615f-94b5-4c62-96f8-b906a3f01ec2"
            }
          ]
        },
        {
          "id": "05c2a126-fe0d-4e7e-b919-af648194abe6",
          "name": "registerEventTopic",
          "request": {
            "url": "http://example.com/api/?Action=RegisterEventTopic?DirectoryId=DirectoryId&TopicName=TopicName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Associates a directory with an SNS topic."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "98628946-eb86-4ca2-b9e5-6a2fc2a75b3b"
            }
          ]
        }
      ]
    },
    {
      "name": "Radius",
      "item": [
        {
          "id": "1efa2b7c-dbf4-4e41-9ad6-8b26c5174bfe",
          "name": "disableRadius",
          "request": {
            "url": "http://example.com/api/?Action=DisableRadius?DirectoryId=DirectoryId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Disables multi-factor authentication (MFA) with the Remote Authentication Dial In User Service (RADIUS) server for an AD Connector directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "02d7f692-dd9d-46ce-ba7f-170ee4deec51"
            }
          ]
        },
        {
          "id": "79ff4dab-3cd4-4fb3-9e84-8f3f12cb2a09",
          "name": "enableRadius",
          "request": {
            "url": "http://example.com/api/?Action=EnableRadius?DirectoryId=DirectoryId&RadiusSettings=RadiusSettings",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Enables multi-factor authentication (MFA) with the Remote Authentication Dial In User Service (RADIUS) server for an AD Connector directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "879855dc-0e05-4c77-aa88-ccafc8c31604"
            }
          ]
        }
      ]
    },
    {
      "name": "SSO",
      "item": [
        {
          "id": "6850004b-3379-448e-8b24-1a1f1a3260ab",
          "name": "disableSso",
          "request": {
            "url": "http://example.com/api/?Action=DisableSso?DirectoryId=DirectoryId&Password=Password&UserName=UserName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Disables single-sign on for a directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "69b306b9-5537-4db7-a96e-f62e41c924bb"
            }
          ]
        },
        {
          "id": "4d7274c6-b705-43a4-bd67-c48a04e718a1",
          "name": "enableSso",
          "request": {
            "url": "http://example.com/api/?Action=EnableSso?DirectoryId=DirectoryId&Password=Password&UserName=UserName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Enables single sign-on for a directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "07674b8f-44bf-4f2c-b5ce-8b78d190659a"
            }
          ]
        }
      ]
    },
    {
      "name": "Schema Extension",
      "item": [
        {
          "id": "e5441975-c29e-4d80-8b1f-2d662bf2b437",
          "name": "listSchemaExtensions",
          "request": {
            "url": "http://example.com/api/?Action=ListSchemaExtensions?DirectoryId=DirectoryId&Limit=Limit&NextToken=NextToken",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all schema extensions applied to a Microsoft AD Directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "501e9749-fae0-49fe-8bb2-c78a4c14806a"
            }
          ]
        },
        {
          "id": "1c1e7e5b-536f-4c8f-8fd3-e9723788842b",
          "name": "startSchemaExtension",
          "request": {
            "url": "http://example.com/api/?Action=StartSchemaExtension?CreateSnapshotBeforeSchemaExtension=CreateSnapshotBeforeSchemaExtension&Description=Description&DirectoryId=DirectoryId&LdifContent=LdifContent",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Applies a schema extension to a Microsoft AD directory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "60fdeae9-d851-4401-af68-b426c1e9ea5a"
            }
          ]
        }
      ]
    }
  ]
}