{
  "info": {
    "name": "AWS Code Pipeline API Get Pipeline Execution",
    "_postman_id": "0d8af922-1e71-4c57-90b1-75c8b87a0c58",
    "description": "Returns information about an execution of a pipeline, including details about\n            artifacts, the pipeline execution ID, and the name, version, and status of the\n            pipeline.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Acknowledge",
      "item": [
        {
          "id": "7f00537b-cb6e-47ce-a354-b9424718c784",
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
              "id": "746bef1d-7c03-4afc-b2f3-bf9aded76d5b"
            }
          ]
        },
        {
          "id": "dba758ae-ec35-457a-8594-e2b40214746e",
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
              "id": "5cdc7a14-911e-48a4-91bd-06cd0bba3aaa"
            }
          ]
        }
      ]
    },
    {
      "name": "Custom",
      "item": [
        {
          "id": "cecf082d-c434-4814-bf1e-baeb79516cae",
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
              "id": "ace377fe-d18b-4b2c-9671-b5fc2822c599"
            }
          ]
        },
        {
          "id": "190b4965-68c3-4f7f-9c7e-202ea93c3144",
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
              "id": "34b5db1f-e938-4a29-af97-39e69859ebba"
            }
          ]
        }
      ]
    },
    {
      "name": "Pipeline",
      "item": [
        {
          "id": "891fd5d6-4df7-4c11-9349-f259d768d5aa",
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
              "id": "f67d1357-2d66-4c9e-b303-886259106415"
            }
          ]
        },
        {
          "id": "abd43f21-d6bc-44e8-9402-bcb5fdca61b5",
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
              "id": "08b83b16-f73f-4a07-86a9-c1ba040304cd"
            }
          ]
        },
        {
          "id": "a5b6c1ce-c1f3-4075-8dba-a45f7a350e89",
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
              "id": "c6b21506-630e-4ab5-972f-8da3f7133a41"
            }
          ]
        },
        {
          "id": "02a4f880-0062-4bd4-afe4-eeb1bf393866",
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
              "id": "5019aa59-7116-41ab-b377-8f68bdb6f498"
            }
          ]
        }
      ]
    },
    {
      "name": "Disable",
      "item": [
        {
          "id": "ebf7e240-2b47-44dc-994c-7ad968b516dc",
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
              "id": "0c2aee36-0daa-4e28-b2e8-78a925a24060"
            }
          ]
        }
      ]
    },
    {
      "name": "Enable",
      "item": [
        {
          "id": "69918baa-1778-4e35-85d3-34a83ff50799",
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
              "id": "b4384710-1a24-49e2-bcfe-8d341a195876"
            }
          ]
        }
      ]
    },
    {
      "name": "Job",
      "item": [
        {
          "id": "e0930cba-32df-404d-9629-64036ce30428",
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
              "id": "6f6dee6c-d259-4e82-946a-49af3a478b5d"
            }
          ]
        }
      ]
    }
  ]
}