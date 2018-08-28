{
  "info": {
    "name": "AWS Code Pipeline API List Pipelines",
    "_postman_id": "bb2fa0be-9084-4031-ba27-3c438b0ff9ec",
    "description": "Gets a summary of all of the pipelines associated with your account.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Acknowledge",
      "item": [
        {
          "id": "f18e2e1a-12e1-4265-afcb-6122d6c6a1a4",
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
              "id": "4f2fc588-7666-4a6c-9ff3-164e87eeef11"
            }
          ]
        },
        {
          "id": "76e3096d-0a9f-47c3-8072-5dd0de483aa1",
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
              "id": "d1a8890d-8796-466c-84ce-aa97782e78ee"
            }
          ]
        }
      ]
    },
    {
      "name": "Custom",
      "item": [
        {
          "id": "cfa60578-42bd-4f56-b50c-4ad9289170fe",
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
              "id": "23f1e96c-7a3c-48f2-b192-f1dad864ffe4"
            }
          ]
        },
        {
          "id": "da7161e7-3c70-467d-8d2f-8f5a077aad13",
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
              "id": "e9d35640-d60e-463a-a8cb-d2780ff442c8"
            }
          ]
        }
      ]
    },
    {
      "name": "Pipeline",
      "item": [
        {
          "id": "caf9ec41-1461-474f-bac1-c89f8f95adf4",
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
              "id": "84685742-f6ec-481b-9010-5bfc0d4be2a9"
            }
          ]
        },
        {
          "id": "2aa533e5-2075-49da-849d-0b280dfd80d0",
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
              "id": "7be96e93-b027-45fa-b5a3-eddc59d79c2e"
            }
          ]
        },
        {
          "id": "066ebe30-0550-4f76-979e-68571aa24796",
          "name": "getPipeline",
          "request": {
            "url": "http://example.com/api/?Action=GetPipeline?Attribute=Attribute&CreateVolumePermission=CreateVolumePermission&DryRun=DryRun&name=name&OperationType=OperationType&SnapshotId=SnapshotId&UserGroup.N=UserGroup.N&UserId.N=UserId.N&version=version",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the metadata, structure, stages, and actions of a pipeline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "38d09073-b45a-4851-a67a-99f1770e4120"
            }
          ]
        },
        {
          "id": "71f5e247-bb7c-4ee9-bc16-b9608bb6edfd",
          "name": "getPipelineExecution",
          "request": {
            "url": "http://example.com/api/?Action=GetPipelineExecution?AutoEnableIO=AutoEnableIO&DryRun=DryRun&pipelineExecutionId=pipelineExecutionId&pipelineName=pipelineName&VolumeId=VolumeId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about an execution of a pipeline, including details about\n            artifacts, the pipeline execution ID, and the name, version, and status of the\n            pipeline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0ccf5b6d-a5eb-4c67-80bf-6b8e28641a58"
            }
          ]
        },
        {
          "id": "8647d87d-3d25-43e9-bbc0-8fcc1da53f0d",
          "name": "getPipelineState",
          "request": {
            "url": "http://example.com/api/?Action=GetPipelineState?Attribute=Attribute&DryRun=DryRun&name=name&SnapshotId=SnapshotId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about the state of a pipeline, including the stages and\n            actions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ce9edc2a-0027-4143-8435-8b90311b60b0"
            }
          ]
        }
      ]
    },
    {
      "name": "Disable",
      "item": [
        {
          "id": "22dca2ba-c494-4e0b-8264-fe4d6db128c2",
          "name": "disableStageTransition",
          "request": {
            "url": "http://example.com/api/?Action=DisableStageTransition?DryRun=DryRun&Filter.N=Filter.N&MaxResults=MaxResults&NextToken=NextToken&pipelineName=pipelineName&reason=reason&stageName=stageName&transitionType=transitionType&VolumeId.N=VolumeId.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Prevents artifacts in a pipeline from transitioning to the next stage in the\n            pipeline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d8b2e119-ec15-4d50-9c6c-8be1c03c46c0"
            }
          ]
        }
      ]
    },
    {
      "name": "Enable",
      "item": [
        {
          "id": "412418f5-93af-40ff-8b06-d9b2b4fdc7b5",
          "name": "enableStageTransition",
          "request": {
            "url": "http://example.com/api/?Action=EnableStageTransition?Device=Device&DryRun=DryRun&Force=Force&InstanceId=InstanceId&pipelineName=pipelineName&stageName=stageName&transitionType=transitionType&VolumeId=VolumeId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Enables artifacts in a pipeline to transition to a stage in a pipeline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5211c37a-1c99-4910-afdc-385b6d4f7fd7"
            }
          ]
        }
      ]
    },
    {
      "name": "Job",
      "item": [
        {
          "id": "cafb7ce3-36ef-4aae-ad7b-3d0c508559fe",
          "name": "getJobDetails",
          "request": {
            "url": "http://example.com/api/?Action=GetJobDetails?DryRun=DryRun&jobId=jobId&VolumeId=VolumeId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about a job."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "01ea2159-c311-4af3-9779-0423cd586ba7"
            }
          ]
        }
      ]
    },
    {
      "name": "Third",
      "item": [
        {
          "id": "a1b8de5a-8b9c-4bc5-b326-b6ff642ff40b",
          "name": "getThirdPartyJobDetails",
          "request": {
            "url": "http://example.com/api/?Action=GetThirdPartyJobDetails?clientToken=clientToken&Domain=Domain&DryRun=DryRun&jobId=jobId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Requests the details of a job for a third party action."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6f13001d-6239-44bf-ad8b-8f2199eec599"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "3792051e-84e1-450d-9d42-53265c837a6b",
          "name": "listActionTypes",
          "request": {
            "url": "http://example.com/api/?Action=ListActionTypes?actionOwnerFilter=actionOwnerFilter&AllocationId=AllocationId&AllowReassociation=AllowReassociation&DryRun=DryRun&InstanceId=InstanceId&NetworkInterfaceId=NetworkInterfaceId&nextToken=nextToken&PrivateIpAddress=PrivateIpAddress&PublicIp=PublicIp",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a summary of all AWS CodePipeline action types associated with your\n            account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c8376e6b-665c-4bc6-a8b9-783af232a332"
            }
          ]
        },
        {
          "id": "073ff433-0a3a-4f5b-9e73-2ee1f802b266",
          "name": "listPipelines",
          "request": {
            "url": "http://example.com/api/?Action=ListPipelines?AllocationId.N=AllocationId.N&DryRun=DryRun&Filter.N=Filter.N&nextToken=nextToken&PublicIp.N=PublicIp.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a summary of all of the pipelines associated with your account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d1476404-30e8-47d5-aef0-3c9493822150"
            }
          ]
        }
      ]
    }
  ]
}