{
  "info": {
    "name": "AWS Data Pipeline API Describe Pipelines",
    "_postman_id": "264c5427-9121-4bae-ad16-647db00e1eb9",
    "description": "Retrieves metadata about one or more pipelines.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Pipeline",
      "item": [
        {
          "id": "99390334-d468-44ff-8519-c161460bb74f",
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
              "id": "e75c4dbf-917d-45ea-8117-998f7fefadf6"
            }
          ]
        },
        {
          "id": "62fcbe44-657b-4f97-919e-5403afe74e43",
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
              "id": "519eed1c-d864-4980-b7a1-2666bb3417c7"
            }
          ]
        },
        {
          "id": "d533e9f9-f377-4221-b810-758a1ab36a86",
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
              "id": "094c0a76-24be-4ce9-91c3-dfadfd8d1bc0"
            }
          ]
        },
        {
          "id": "8f4dc673-5ab2-4f81-8e49-56c2cc0c45ea",
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
              "id": "f5df188a-bce5-4de2-9d0e-991942d704dc"
            }
          ]
        },
        {
          "id": "d9561e4d-efa3-4348-9c2f-50a7ad49a820",
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
              "id": "9e43daa2-26a4-41c6-aff5-6b2e3d20a3bf"
            }
          ]
        }
      ]
    },
    {
      "name": "Tags",
      "item": [
        {
          "id": "e721a5ac-590d-47db-a311-4689ba17479f",
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
              "id": "3c399619-7cd9-47c7-b0b5-7219ffe8618c"
            }
          ]
        }
      ]
    },
    {
      "name": "Objects",
      "item": [
        {
          "id": "8dbb0441-cfb1-483b-aff7-6d721549d198",
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
              "id": "9210d60e-b282-4d47-9bd5-f0da8868321e"
            }
          ]
        }
      ]
    }
  ]
}