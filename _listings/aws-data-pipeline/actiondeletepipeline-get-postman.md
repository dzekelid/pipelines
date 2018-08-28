{
  "info": {
    "name": "AWS Data Pipeline API Delete Pipeline",
    "_postman_id": "4b7ae612-c2a8-4c60-ba01-5422cb4ad4da",
    "description": "Deletes a pipeline, its pipeline definition, and its run history.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Pipeline",
      "item": [
        {
          "id": "516b48af-888c-4343-a7f8-15e58602c3d6",
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
              "id": "656d2dbf-cebc-4474-90e8-3adeb4289e68"
            }
          ]
        },
        {
          "id": "40e088ff-30e4-4bbc-ad24-251410840065",
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
              "id": "7d8953c3-b40f-40fc-80fc-82682d0dfcb5"
            }
          ]
        },
        {
          "id": "799db090-7081-44a5-b377-87c9bac0ef38",
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
              "id": "af8fe012-1c64-4e04-a9b9-35bb844a72cd"
            }
          ]
        },
        {
          "id": "cb4be731-61c8-4382-b98c-edf9350d7d16",
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
              "id": "8cf3f71a-c55e-4d78-8229-69ab9c03095b"
            }
          ]
        }
      ]
    },
    {
      "name": "Tags",
      "item": [
        {
          "id": "00cabfca-4349-4590-a252-b331bcaf7337",
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
              "id": "38e03af9-c7b1-452b-86a3-b035bbd45df6"
            }
          ]
        }
      ]
    }
  ]
}