{
  "info": {
    "name": "AWS Code Pipeline API Start Pipeline Execution",
    "_postman_id": "25b9e936-c674-41a0-b710-845038ddc3a9",
    "description": "Starts the specified pipeline.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Acknowledge",
      "item": [
        {
          "id": "c7fdba84-44ed-40b5-8293-92c2ddcbb9de",
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
              "id": "430cc73c-9c81-45ae-b50e-f64320533074"
            }
          ]
        },
        {
          "id": "59ab14f3-6ad1-406a-b416-14bd40131ea0",
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
              "id": "15a4fe81-dfa7-479c-9fb2-b0ddff9f3601"
            }
          ]
        }
      ]
    },
    {
      "name": "Custom",
      "item": [
        {
          "id": "664670a9-0a92-4548-8743-b8eecec02a87",
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
              "id": "ef979126-7143-4243-847b-bd9c6bdc0081"
            }
          ]
        },
        {
          "id": "6b10edb5-ae4d-44f2-bfae-98d6425267be",
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
              "id": "3989bfd8-a7c6-4181-ad98-1f2e07ccfe87"
            }
          ]
        }
      ]
    },
    {
      "name": "Pipeline",
      "item": [
        {
          "id": "3400c8f7-632c-48e0-ae89-0bbc653f9f90",
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
              "id": "fb7b0698-da09-4be6-9957-2e227bcf6c1e"
            }
          ]
        },
        {
          "id": "219139d0-8fd2-4362-b9e4-9c6875e6a3ff",
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
              "id": "68b3344e-c398-46e9-8abe-5fe33b632faf"
            }
          ]
        },
        {
          "id": "c3201e58-fb9b-4a68-aeb5-4711bcad83c1",
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
              "id": "20e3d269-6dbb-41a8-8435-6104662d4ccd"
            }
          ]
        },
        {
          "id": "aee7ae08-e7d4-466a-823b-76d795fc25bb",
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
              "id": "2f3e18bf-d77c-4ab9-89a0-fe89d22f66e4"
            }
          ]
        },
        {
          "id": "d0cd6fc6-b126-4327-bc22-88d0dbdc1001",
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
              "id": "5b909445-4b21-40f8-95fa-965221a08c2b"
            }
          ]
        }
      ]
    },
    {
      "name": "Disable",
      "item": [
        {
          "id": "f1c9cd8a-cdce-4653-aeb4-db04b35ee7c1",
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
              "id": "2f8a7930-a0d5-4b92-a5f7-57768a23e868"
            }
          ]
        }
      ]
    },
    {
      "name": "Enable",
      "item": [
        {
          "id": "1b0d86cc-cd44-4f89-8344-263b29b4c4d4",
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
              "id": "0adf0cff-ac4b-4205-a7b7-4b64836d6d3c"
            }
          ]
        }
      ]
    },
    {
      "name": "Job",
      "item": [
        {
          "id": "3d031ad1-f5b4-46b1-b19b-824f254b7acf",
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
              "id": "09294052-a504-4335-adcf-00d183191ee7"
            }
          ]
        }
      ]
    },
    {
      "name": "Third",
      "item": [
        {
          "id": "f7f519dc-08f7-4a92-a9d2-0c449bb135aa",
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
              "id": "70cb1e8a-c7d8-4edb-bb3f-4cd123b5128d"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "549f4f34-40e2-4754-b521-0b0126bccdbe",
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
              "id": "8022eb4e-8beb-4a58-acd4-a178ef5f42ff"
            }
          ]
        },
        {
          "id": "0e13127c-77ea-4d01-919d-8758c642e67c",
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
              "id": "1986e226-47c9-4aa1-899c-b269ed690e4e"
            }
          ]
        }
      ]
    },
    {
      "name": "PollJobs",
      "item": [
        {
          "id": "615de587-cfe3-4f73-a76a-143a5b105f62",
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
              "id": "3b839c8f-ad88-4610-94d1-f6fecc369a4c"
            }
          ]
        }
      ]
    },
    {
      "name": "PollThird",
      "item": [
        {
          "id": "b2f5b8d0-58f9-4d24-8c3f-c264c969c8cb",
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
              "id": "bd2e3cff-6719-4e1d-ad76-f3cbd13bccd2"
            }
          ]
        }
      ]
    },
    {
      "name": "Put",
      "item": [
        {
          "id": "de1c5a22-ef7f-4b85-86c7-cb9208a0d176",
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
              "id": "28694a29-d7e9-4b5c-af5d-cbc4ff8ae461"
            }
          ]
        },
        {
          "id": "f5d07f1e-bf76-4b84-a3a6-91dfbf4ba828",
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
              "id": "caf29713-9d69-464b-8e19-fccc488a0e15"
            }
          ]
        },
        {
          "id": "a7275bbc-0e16-4535-afdd-7c7618e72324",
          "name": "putJobFailureResult",
          "request": {
            "url": "http://example.com/api/?Action=PutJobFailureResult?DryRun=DryRun&failureDetails=failureDetails&jobId=jobId&PublicIp=PublicIp",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Represents the failure of a job as returned to the pipeline by a job worker."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3e39d380-ba53-40b6-8129-246a506fdc9e"
            }
          ]
        },
        {
          "id": "ddada303-fb57-47d4-89e1-40ca74c938d8",
          "name": "putJobSuccessResult",
          "request": {
            "url": "http://example.com/api/?Action=PutJobSuccessResult?continuationToken=continuationToken&currentRevision=currentRevision&executionDetails=executionDetails&Ipv6AddressCount=Ipv6AddressCount&Ipv6Addresses.N=Ipv6Addresses.N&jobId=jobId&NetworkInterfaceId=NetworkInterfaceId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Represents the success of a job as returned to the pipeline by a job worker."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "838f0d63-68b7-48ad-a797-e821bea5662b"
            }
          ]
        },
        {
          "id": "e3b40f72-62da-4487-9ed8-9e5ff44548fd",
          "name": "putThirdPartyJobFailureResult",
          "request": {
            "url": "http://example.com/api/?Action=PutThirdPartyJobFailureResult?AllowReassignment=AllowReassignment&clientToken=clientToken&failureDetails=failureDetails&jobId=jobId&NetworkInterfaceId=NetworkInterfaceId&PrivateIpAddress.N=PrivateIpAddress.N&SecondaryPrivateIpAddressCount=SecondaryPrivateIpAddressCount",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Represents the failure of a third party job as returned to the pipeline by a job\n            worker."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "be52dae0-b3a6-4b78-9b92-35ccb6e1f7f3"
            }
          ]
        },
        {
          "id": "43cd4b7a-2ecf-4c9c-b310-f2325318eb91",
          "name": "putThirdPartyJobSuccessResult",
          "request": {
            "url": "http://example.com/api/?Action=PutThirdPartyJobSuccessResult?clientToken=clientToken&continuationToken=continuationToken&currentRevision=currentRevision&DeviceIndex=DeviceIndex&DryRun=DryRun&executionDetails=executionDetails&InstanceId=InstanceId&jobId=jobId&NetworkInterfaceId=NetworkInterfaceId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Represents the success of a third party job as returned to the pipeline by a job\n            worker."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6d8ea5df-26db-4c36-b17c-3036cbb27d94"
            }
          ]
        }
      ]
    },
    {
      "name": "Retry",
      "item": [
        {
          "id": "7953b03e-8bb9-4dc2-b972-e8cf7534edd8",
          "name": "retryStageExecution",
          "request": {
            "url": "http://example.com/api/?Action=RetryStageExecution?Description=Description&DryRun=DryRun&Ipv6AddressCount=Ipv6AddressCount&Ipv6Addresses.N=Ipv6Addresses.N&pipelineExecutionId=pipelineExecutionId&pipelineName=pipelineName&PrivateIpAddress=PrivateIpAddress&PrivateIpAddresses.N=PrivateIpAddresses.N&retryMode=retryMode&SecondaryPrivateIpAddressCount=SecondaryPrivateIpAddressCount&SecurityGroupId.N=SecurityGroupId.N&stageName=stageName&SubnetId=SubnetId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Resumes the pipeline execution by retrying the last failed actions in a\n            stage."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "177c74a3-2cff-4dc0-a7c7-b1e846590c28"
            }
          ]
        }
      ]
    },
    {
      "name": "Start",
      "item": [
        {
          "id": "fecba5ed-16cf-4e0e-a424-e2c4ad7e0296",
          "name": "startPipelineExecution",
          "request": {
            "url": "http://example.com/api/?Action=StartPipelineExecution?DryRun=DryRun&name=name&NetworkInterfaceId=NetworkInterfaceId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Starts the specified pipeline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "74fb34fa-b4d7-4760-8a48-c05ee5624449"
            }
          ]
        }
      ]
    }
  ]
}