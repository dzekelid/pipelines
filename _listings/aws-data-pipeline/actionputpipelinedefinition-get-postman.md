{
  "info": {
    "name": "AWS Data Pipeline API Put Pipeline Definition",
    "_postman_id": "a5f3c7f6-b721-42b4-937b-dd0575e8d3b7",
    "description": "Adds tasks, schedules, and preconditions to the specified pipeline.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Pipeline",
      "item": [
        {
          "id": "72de2520-b2c4-4ecf-8cb4-0bc886d67c87",
          "name": "activatePipeline",
          "request": {
            "url": "http://example.com/api/?Action=ActivatePipeline?parameterValues=parameterValues&pipelineId=pipelineId&startTimestamp=startTimestamp",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Validates the specified pipeline and starts processing pipeline tasks."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "722b4ba2-2f55-43b7-98a8-14066afc1e57"
            }
          ]
        },
        {
          "id": "72a5498a-8892-4da3-bcdc-ab3a41908ff4",
          "name": "createPipeline",
          "request": {
            "url": "http://example.com/api/?Action=CreatePipeline?description=description&name=name&tags=tags&uniqueId=uniqueId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new, empty pipeline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a3c666e5-e5d1-4998-b968-fe26698f8f24"
            }
          ]
        },
        {
          "id": "3a1eea60-b232-4cdf-acab-e08cb8238436",
          "name": "deactivatePipeline",
          "request": {
            "url": "http://example.com/api/?Action=DeactivatePipeline?cancelActive=cancelActive&pipelineId=pipelineId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deactivates the specified running pipeline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d9643217-f178-44b2-9877-b9a6a3258516"
            }
          ]
        },
        {
          "id": "ed34e212-5f3e-43e2-9443-41f87c66ddca",
          "name": "deletePipeline",
          "request": {
            "url": "http://example.com/api/?Action=DeletePipeline?pipelineId=pipelineId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a pipeline, its pipeline definition, and its run history."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f2b73862-b4d4-4929-9b0b-b849328392fe"
            }
          ]
        },
        {
          "id": "ecb240f4-d5ec-4bba-978d-b4a4c2f6cbb4",
          "name": "describePipelines",
          "request": {
            "url": "http://example.com/api/?Action=DescribePipelines?pipelineIds=pipelineIds",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves metadata about one or more pipelines."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c3e8ab62-01d1-4d53-a5ec-e3d749135b26"
            }
          ]
        },
        {
          "id": "e89bd2d2-5c6a-469b-81e0-cf6705352d18",
          "name": "getPipelineDefinition",
          "request": {
            "url": "http://example.com/api/?Action=GetPipelineDefinition?pipelineId=pipelineId&version=version",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the definition of the specified pipeline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bbd1103e-1f07-40db-bf38-ddcb8574467c"
            }
          ]
        },
        {
          "id": "092f6521-b07c-4f54-95b8-4e3618570ded",
          "name": "listPipelines",
          "request": {
            "url": "http://example.com/api/?Action=ListPipelines?marker=marker",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the pipeline identifiers for all active pipelines that you have permission to access."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3c71c42b-fc55-4412-9c96-b70b64e98d56"
            }
          ]
        },
        {
          "id": "c4eaa3ea-6db1-443d-8024-431929dcfd04",
          "name": "putPipelineDefinition",
          "request": {
            "url": "http://example.com/api/?Action=PutPipelineDefinition?parameterObjects=parameterObjects&parameterValues=parameterValues&pipelineId=pipelineId&pipelineObjects=pipelineObjects",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds tasks, schedules, and preconditions to the specified pipeline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "16403bd4-2183-46b9-b812-5ace73d03247"
            }
          ]
        }
      ]
    },
    {
      "name": "Tags",
      "item": [
        {
          "id": "b9a54c79-1496-4c8e-8eb8-904c5606204d",
          "name": "addTags",
          "request": {
            "url": "http://example.com/api/?Action=AddTags?pipelineId=pipelineId&tags=tags",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Adds or modifies tags for the specified pipeline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1f4618d4-fb80-44ff-8070-17e15d9b4c74"
            }
          ]
        }
      ]
    },
    {
      "name": "Objects",
      "item": [
        {
          "id": "cdbba6e2-973e-4e2e-9a6b-4a4298cd9c8f",
          "name": "describeObjects",
          "request": {
            "url": "http://example.com/api/?Action=DescribeObjects?evaluateExpressions=evaluateExpressions&marker=marker&objectIds=objectIds&pipelineId=pipelineId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the object definitions for a set of objects associated with the pipeline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "af0026d4-b9b1-4abd-8839-e20a1c5f583b"
            }
          ]
        }
      ]
    },
    {
      "name": "Expressions",
      "item": [
        {
          "id": "458e8369-2842-440f-abb9-35942e6af4e3",
          "name": "evaluateExpression",
          "request": {
            "url": "http://example.com/api/?Action=EvaluateExpression?expression=expression&objectId=objectId&pipelineId=pipelineId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Task runners call EvaluateExpression to evaluate a string in the context of the specified object."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ae1ffefb-1acd-42a8-8388-3377bc342452"
            }
          ]
        }
      ]
    },
    {
      "name": "Tasks",
      "item": [
        {
          "id": "024bcd68-1cd9-4337-a6b7-7c24f8b3f052",
          "name": "pollForTask",
          "request": {
            "url": "http://example.com/api/?Action=PollForTask?hostname=hostname&instanceIdentity=instanceIdentity&workerGroup=workerGroup",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Task runners call PollForTask to receive a task to perform from AWS Data Pipeline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0a0fe9c2-ec40-4113-9586-535f8dcd3216"
            }
          ]
        }
      ]
    }
  ]
}