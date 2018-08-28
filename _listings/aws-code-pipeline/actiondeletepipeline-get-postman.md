{
  "info": {
    "name": "AWS Code Pipeline API Delete Pipeline",
    "_postman_id": "4bca6ca6-3250-4186-b6ff-0e86a432a991",
    "description": "Deletes the specified pipeline.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Acknowledge",
      "item": [
        {
          "id": "cff7b2ba-6f1e-4f3f-a237-818ad527fee9",
          "name": "acknowledgeJob",
          "request": {
            "url": "http://example.com/api/?Action=AcknowledgeJob?DryRun=DryRun&jobId=jobId&nonce=nonce&SnapshotId=SnapshotId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about a specified job and whether that job has been received by\n            the job worker."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8a576dba-b89e-4c6a-bc0d-176a432ad09b"
            }
          ]
        },
        {
          "id": "2922acae-0e26-4691-bc39-e07d3c6e405f",
          "name": "acknowledgeThirdPartyJob",
          "request": {
            "url": "http://example.com/api/?Action=AcknowledgeThirdPartyJob?clientToken=clientToken&DryRun=DryRun&jobId=jobId&nonce=nonce&VolumeId=VolumeId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Confirms a job worker has received the specified job."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c41cb2aa-539c-4323-8df3-c0c9f5ae232a"
            }
          ]
        }
      ]
    },
    {
      "name": "Custom",
      "item": [
        {
          "id": "4ff42ab4-0976-4e8b-bfff-95b6a4a73867",
          "name": "createCustomActionType",
          "request": {
            "url": "http://example.com/api/?Action=CreateCustomActionType?Attribute=Attribute&category=category&configurationProperties=configurationProperties&DryRun=DryRun&inputArtifactDetails=inputArtifactDetails&outputArtifactDetails=outputArtifactDetails&provider=provider&settings=settings&SnapshotId=SnapshotId&version=version",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new custom action that can be used in all pipelines associated with the\n            AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "87f97586-5d27-46a0-b704-831e65242b9e"
            }
          ]
        },
        {
          "id": "3ac01a8d-867a-48ec-ac1b-f41375448ecf",
          "name": "deleteCustomActionType",
          "request": {
            "url": "http://example.com/api/?Action=DeleteCustomActionType?Attribute=Attribute&category=category&DryRun=DryRun&provider=provider&version=version&VolumeId=VolumeId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Marks a custom action as deleted."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bc37c048-5dc5-4843-8481-e4070128db02"
            }
          ]
        }
      ]
    },
    {
      "name": "Pipeline",
      "item": [
        {
          "id": "53efddee-9601-4f1c-8419-6964b5160f1f",
          "name": "createPipeline",
          "request": {
            "url": "http://example.com/api/?Action=CreatePipeline?DryRun=DryRun&Filter.N=Filter.N&MaxResults=MaxResults&NextToken=NextToken&Owner.N=Owner.N&pipeline=pipeline&RestorableBy.N=RestorableBy.N&SnapshotId.N=SnapshotId.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a pipeline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1c508d74-6f7f-475a-ad70-4785bf707e31"
            }
          ]
        },
        {
          "id": "e2b36b1d-f4a1-4492-baa7-48e3c28606cc",
          "name": "deletePipeline",
          "request": {
            "url": "http://example.com/api/?Action=DeletePipeline?DryRun=DryRun&Filter.N=Filter.N&MaxResults=MaxResults&name=name&NextToken=NextToken&VolumeId.N=VolumeId.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified pipeline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "80380ac7-335d-4f5d-ae70-be25223a8246"
            }
          ]
        }
      ]
    }
  ]
}