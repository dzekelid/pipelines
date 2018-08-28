{
  "info": {
    "name": "AWS Data Pipeline API Get Pipeline Definition",
    "_postman_id": "bd9716d2-7a4f-476b-8693-402d9c4b910a",
    "description": "Gets the definition of the specified pipeline.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Pipeline",
      "item": [
        {
          "id": "657917dc-e063-4c7a-bb6b-70b2ed78e354",
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
              "id": "dc45c1e8-a958-4952-91f8-a44fdb912ac0"
            }
          ]
        },
        {
          "id": "ae552dd2-a7ed-428c-b0dc-fdcdc9d4855d",
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
              "id": "82e4b1ce-0524-4029-a421-27d4ddedd920"
            }
          ]
        },
        {
          "id": "87d525f7-c2c7-44dc-9dfd-b2d0770deffe",
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
              "id": "0ec64987-15c4-4fb2-994b-7bdbc1a7ee1b"
            }
          ]
        },
        {
          "id": "670b12e0-aadd-4718-a9b4-36934aabf282",
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
              "id": "da7a7c55-ca3c-492b-94be-c1af69a84631"
            }
          ]
        },
        {
          "id": "4c281c61-00da-4cd6-8f07-95925d25755e",
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
              "id": "597703bc-704b-4c0e-97b3-71f0a62bbb1b"
            }
          ]
        },
        {
          "id": "2a556d1e-c009-456a-8d71-e5c8a07b77e0",
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
              "id": "1f1576a4-fede-43a7-8b1e-d8af54b00171"
            }
          ]
        }
      ]
    },
    {
      "name": "Tags",
      "item": [
        {
          "id": "2cc734a9-afc7-43d6-bed2-a02ced2d4670",
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
              "id": "22f18f7b-a878-40e9-a935-cacb1affbcaa"
            }
          ]
        }
      ]
    },
    {
      "name": "Objects",
      "item": [
        {
          "id": "be6c955b-7cf6-46df-832a-6fd1dc4442e4",
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
              "id": "3cec2185-e79f-4650-a262-119cf66ac5b2"
            }
          ]
        }
      ]
    },
    {
      "name": "Expressions",
      "item": [
        {
          "id": "f5f2c458-ead9-4673-b0ee-f88b29991e76",
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
              "id": "aadc5ae8-547c-44ee-a78a-37fb0ece6534"
            }
          ]
        }
      ]
    }
  ]
}