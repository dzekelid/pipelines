{
  "info": {
    "name": "AWS Data Pipeline API Deactivate Pipeline",
    "_postman_id": "d8bcbd78-88cd-485b-b726-f10daab3c9e2",
    "description": "Deactivates the specified running pipeline.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Pipeline",
      "item": [
        {
          "id": "14b5d082-e897-49a8-b311-2f129a869824",
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
              "id": "cfed3b6a-a796-4b7b-b90c-3f1a2de71bf9"
            }
          ]
        },
        {
          "id": "7eca10ff-de50-4527-8cf0-5ef700ad2fa0",
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
              "id": "eb2e8610-d852-4ce9-823c-01497de40ac9"
            }
          ]
        },
        {
          "id": "847a6c0c-dd43-4919-9116-6273b09ebb25",
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
              "id": "6b94a5ec-e6b2-442f-bdcb-a3ebae6304ec"
            }
          ]
        }
      ]
    },
    {
      "name": "Tags",
      "item": [
        {
          "id": "847babbb-940b-460d-919a-b2c4d2510ec8",
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
              "id": "51304e20-2254-471d-9d72-13836c6cf0ce"
            }
          ]
        }
      ]
    }
  ]
}