{
  "info": {
    "name": "AWS Code Pipeline API Put Action Revision",
    "_postman_id": "8ef9ecd4-b303-4eba-99c7-b52b8f416fc2",
    "description": "Provides information to AWS CodePipeline about new revisions to a source.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Acknowledge",
      "item": [
        {
          "id": "7dd22b89-57af-4739-82ce-af5ed44d83db",
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
              "id": "962c81eb-8325-4279-a20a-9f0b03025f84"
            }
          ]
        },
        {
          "id": "b890ad91-f99f-44f2-947f-edd579974a81",
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
              "id": "ce964f05-e282-4156-afd8-a52b54b0f357"
            }
          ]
        }
      ]
    },
    {
      "name": "Custom",
      "item": [
        {
          "id": "1440db28-e4fd-4659-8de6-011ca26b5700",
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
              "id": "358a8783-644f-4a5c-aaf9-e68ba97b5b33"
            }
          ]
        },
        {
          "id": "14501719-f87d-4d78-9a4a-aef9f27400ff",
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
              "id": "3fb18312-c915-459b-8a43-00d73c67184c"
            }
          ]
        }
      ]
    },
    {
      "name": "Pipeline",
      "item": [
        {
          "id": "49dd70b7-5134-4152-ba48-4cb289e4d14a",
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
              "id": "b1ecfc12-7d7f-4898-a5e5-2b324d4f78df"
            }
          ]
        },
        {
          "id": "d611ee77-ad64-44e3-9c1f-2fb5d54914b7",
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
              "id": "c37b1127-f478-478c-be6c-63ca2e1982a4"
            }
          ]
        },
        {
          "id": "60d3ffcb-6945-4b44-9263-1d2d05b39238",
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
              "id": "24a61e2b-66d5-40af-8a41-429c5d716318"
            }
          ]
        },
        {
          "id": "a9c469cd-1737-4db7-a884-3ecc7178209d",
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
              "id": "aeb2ecd4-b794-438e-a7ef-441878746262"
            }
          ]
        },
        {
          "id": "657a2b9f-e851-4be5-9540-3fa635717825",
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
              "id": "a030fc52-5b66-4e65-9f09-e8c6799dac17"
            }
          ]
        }
      ]
    },
    {
      "name": "Disable",
      "item": [
        {
          "id": "59313368-0f43-40fe-9c5e-8e6ca1384e7e",
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
              "id": "a38b9994-4ca6-4613-99d3-6177fba8fdea"
            }
          ]
        }
      ]
    },
    {
      "name": "Enable",
      "item": [
        {
          "id": "e162e907-77df-4a06-93d6-b8e3b1c2b9db",
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
              "id": "cfaaee0f-a8e2-4e6f-ae2a-4e4b6dd9d608"
            }
          ]
        }
      ]
    },
    {
      "name": "Job",
      "item": [
        {
          "id": "44608dbf-6b35-4418-b3fd-459c81bdac2f",
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
              "id": "9c9d33b6-c7b9-4835-8021-9cbb50d9473a"
            }
          ]
        }
      ]
    },
    {
      "name": "Third",
      "item": [
        {
          "id": "40a55511-8561-4294-973e-61c0c6c10f0a",
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
              "id": "02ce2abb-5c71-40f8-83cb-79434069a0c5"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "d2103e11-0a98-4297-9d25-985fced94776",
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
              "id": "53b12b49-d23e-4a7b-9f25-7d35c469855d"
            }
          ]
        },
        {
          "id": "8d93bbb7-81cc-4441-acc0-7f9d218d6e9d",
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
              "id": "2b8d9412-b2e1-4259-b403-a762090d6242"
            }
          ]
        }
      ]
    },
    {
      "name": "PollJobs",
      "item": [
        {
          "id": "78b511d7-969c-4474-af52-f056d42446c7",
          "name": "pollForJobs",
          "request": {
            "url": "http://example.com/api/?Action=PollForJobs?actionTypeId=actionTypeId&DryRun=DryRun&Filter.N=Filter.N&maxBatchSize=maxBatchSize&MaxResults=MaxResults&NextToken=NextToken&PublicIp.N=PublicIp.N&queryParam=queryParam",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about any jobs for AWS CodePipeline to act upon."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "03893199-c2bf-462e-9ab8-df04096e8cf4"
            }
          ]
        }
      ]
    },
    {
      "name": "PollThird",
      "item": [
        {
          "id": "cb623b59-308a-411e-a987-3c380ad2caa5",
          "name": "pollForThirdPartyJobs",
          "request": {
            "url": "http://example.com/api/?Action=PollForThirdPartyJobs?actionTypeId=actionTypeId&AssociationId=AssociationId&DryRun=DryRun&maxBatchSize=maxBatchSize&PublicIp=PublicIp",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Determines whether there are any third party jobs for a job worker to act on."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "00193a29-b095-48f8-a209-84d366068359"
            }
          ]
        }
      ]
    },
    {
      "name": "Put",
      "item": [
        {
          "id": "f42d769f-7336-4923-8188-92ca7abd74e4",
          "name": "putActionRevision",
          "request": {
            "url": "http://example.com/api/?Action=PutActionRevision?actionName=actionName&actionRevision=actionRevision&DryRun=DryRun&pipelineName=pipelineName&PublicIp=PublicIp&stageName=stageName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Provides information to AWS CodePipeline about new revisions to a source."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c622c4d3-ab71-4db9-a6b0-702611f96dbf"
            }
          ]
        }
      ]
    }
  ]
}