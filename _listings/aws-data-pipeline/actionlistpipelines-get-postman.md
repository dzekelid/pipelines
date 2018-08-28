{
  "info": {
    "name": "AWS Data Pipeline API List Pipelines",
    "_postman_id": "69ed3a82-f5e1-4f79-9b8a-78ab19a214ee",
    "description": "Lists the pipeline identifiers for all active pipelines that you have permission to access.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Pipeline",
      "item": [
        {
          "id": "d480f59a-eae3-465f-9513-7e32c984706f",
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
              "id": "8fa5a2d5-6cd9-4f8e-bbcc-72cd8f2698b7"
            }
          ]
        },
        {
          "id": "86a7e39a-e8cc-45fd-b346-553cdd2ddd6e",
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
              "id": "6cd0242d-8475-45b5-987c-c48f5cfdcaa5"
            }
          ]
        },
        {
          "id": "d5cdfbc1-fe88-4796-9d0d-1b8108bb8dd2",
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
              "id": "b6fe1b0c-36e5-447a-9088-a8c3c8f60f26"
            }
          ]
        },
        {
          "id": "a20da1bf-3d44-441d-b184-ec5984ccd313",
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
              "id": "48e828bb-04f9-4c86-a188-74cb96f78332"
            }
          ]
        },
        {
          "id": "a5601359-73f0-45ff-8702-cf722c56ee0a",
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
              "id": "a2ff7860-6ebb-43da-afea-ea8ed7317dbf"
            }
          ]
        },
        {
          "id": "57c17d79-5160-41b8-aa16-1e3e4efbb1c5",
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
              "id": "3d1421dd-b5a7-4062-8086-a26f357cff85"
            }
          ]
        },
        {
          "id": "6b2f2795-ee5a-44e2-8e99-0352d86a74b5",
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
              "id": "4a2e1397-9322-436f-9d71-4593a7dad1ba"
            }
          ]
        }
      ]
    },
    {
      "name": "Tags",
      "item": [
        {
          "id": "8196d146-2e64-464a-ad16-57ba1268a213",
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
              "id": "be0481f4-e778-46d5-9b19-3745556917ba"
            }
          ]
        }
      ]
    },
    {
      "name": "Objects",
      "item": [
        {
          "id": "cfd71eea-5ba9-4347-b095-62f6cb151040",
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
              "id": "c051bb29-fb7f-462e-bc7a-5095702c8ab8"
            }
          ]
        }
      ]
    },
    {
      "name": "Expressions",
      "item": [
        {
          "id": "f95be5e4-27c1-4cdf-b1fb-3c435cd6f7b0",
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
              "id": "3a4fef35-4ac9-4467-99f1-3582a094b0d1"
            }
          ]
        }
      ]
    }
  ]
}