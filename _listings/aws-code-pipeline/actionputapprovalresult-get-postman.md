{
  "info": {
    "name": "AWS Code Pipeline API Put Approval Result",
    "_postman_id": "1ca6d853-b746-44e7-8b94-915b4bbe6f08",
    "description": "Provides the response to a manual approval request to AWS CodePipeline.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Acknowledge",
      "item": [
        {
          "id": "f8bd3b59-9e0a-48aa-abc5-3f1d4ad0b9e5",
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
              "id": "84f06d36-959c-4d38-ac96-cb458ea8e487"
            }
          ]
        },
        {
          "id": "b36a88ae-14d1-4a89-bd89-311e88f915d6",
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
              "id": "007778bf-46e0-4bf7-b6f4-7af0ab0062bf"
            }
          ]
        }
      ]
    },
    {
      "name": "Custom",
      "item": [
        {
          "id": "7ffc6b75-825d-4f53-938c-c1aacc292d56",
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
              "id": "95c2d9c1-d5cf-4bd1-af17-d720a55540c7"
            }
          ]
        },
        {
          "id": "8c689825-5f77-4967-a3e6-97fe20475660",
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
              "id": "84cf3844-9791-4500-9470-643fdc3a27b3"
            }
          ]
        }
      ]
    },
    {
      "name": "Pipeline",
      "item": [
        {
          "id": "0481d15a-94ce-40e0-9aa2-9a05efb04a9b",
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
              "id": "052554c2-b61c-48e4-8cab-682b2822f941"
            }
          ]
        },
        {
          "id": "2857008f-ce24-4fad-9e0a-428a5869a8f4",
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
              "id": "4dffe6a5-2ae9-4f7c-b365-d13988dfa989"
            }
          ]
        },
        {
          "id": "2a1a806e-eec9-45d2-b0f9-1dc626fde39d",
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
              "id": "1b1a7075-a5dc-4ed2-947e-5fe449cb8244"
            }
          ]
        },
        {
          "id": "fc03480c-9624-4e41-8f03-0c3c00492e22",
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
              "id": "fefbcb42-caa8-491e-bdac-434a4db6ff23"
            }
          ]
        },
        {
          "id": "47a553d6-b473-43fb-a34b-2ddbbb3aed10",
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
              "id": "5e294b2a-0f22-411d-b629-7fa8ce872050"
            }
          ]
        }
      ]
    },
    {
      "name": "Disable",
      "item": [
        {
          "id": "74468f9a-b463-4151-a711-60a653007d7b",
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
              "id": "f09cc39a-a9e0-4fe7-981d-748f6514b0c1"
            }
          ]
        }
      ]
    },
    {
      "name": "Enable",
      "item": [
        {
          "id": "d3b2e924-13fc-478f-96e5-af5469efe77d",
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
              "id": "4d91c0bf-5ba4-4aa6-a7dd-37952b1fcfd0"
            }
          ]
        }
      ]
    },
    {
      "name": "Job",
      "item": [
        {
          "id": "ec9cd92f-8314-4d51-a8cd-d0191ef445fd",
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
              "id": "78f4b5dc-f137-448a-b54b-71b4b3e15705"
            }
          ]
        }
      ]
    },
    {
      "name": "Third",
      "item": [
        {
          "id": "d6768c53-6f43-430e-967d-6bd8c8d5685f",
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
              "id": "9615109b-5bdd-4d76-9086-1c4b1310c4a4"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "4ac18019-6e56-47a1-a914-11ab2e988cd2",
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
              "id": "94dca211-0691-41cd-ba48-3d6b8a76b5a5"
            }
          ]
        },
        {
          "id": "2d960ab6-e282-4584-854d-47e53a6fc70f",
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
              "id": "8493a9d8-b4de-4e60-a34c-64ceacf76bd5"
            }
          ]
        }
      ]
    },
    {
      "name": "PollJobs",
      "item": [
        {
          "id": "689cbe3e-4469-4c0f-a82f-84bd8e8727b4",
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
              "id": "910730a2-71a2-4f37-a510-6b13394f7d3d"
            }
          ]
        }
      ]
    },
    {
      "name": "PollThird",
      "item": [
        {
          "id": "67cf05d6-7eb2-4910-8f22-87554094b7d4",
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
              "id": "a7b1eb2e-3806-4d05-93cd-a09494c08ecf"
            }
          ]
        }
      ]
    },
    {
      "name": "Put",
      "item": [
        {
          "id": "e892ddd2-800a-4202-b757-6421bd0538e0",
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
              "id": "98d0dd43-0974-4422-8277-f32e58a7f34d"
            }
          ]
        },
        {
          "id": "39112aa4-3aa4-4b5d-a0ee-dafa8238ad3c",
          "name": "putApprovalResult",
          "request": {
            "url": "http://example.com/api/?Action=PutApprovalResult?actionName=actionName&AllocationId=AllocationId&DryRun=DryRun&pipelineName=pipelineName&PublicIp=PublicIp&result=result&stageName=stageName&token=token",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Provides the response to a manual approval request to AWS CodePipeline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "360c211a-a1cc-4147-b8bd-1daf96292519"
            }
          ]
        }
      ]
    }
  ]
}