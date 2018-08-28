{
  "info": {
    "name": "AWS Data Pipeline API Create Pipeline",
    "_postman_id": "7fb34d79-ce30-41d7-b4a9-7d7128be303d",
    "description": "Creates a new, empty pipeline.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Pipeline",
      "item": [
        {
          "id": "3e0c547b-3f4f-4d77-9038-88c536feabce",
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
              "id": "e00defbb-2ca9-4041-902c-0c734ebba04b"
            }
          ]
        },
        {
          "id": "9a26e275-2d4d-43aa-981f-44e567a1dc38",
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
              "id": "fd155709-a1a0-4374-b42e-5630393badc1"
            }
          ]
        }
      ]
    },
    {
      "name": "Tags",
      "item": [
        {
          "id": "88084692-297f-4cd8-a0a6-0918e02d6e83",
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
              "id": "f4eb50aa-ca79-4b53-b6e0-b4260321e2bd"
            }
          ]
        }
      ]
    }
  ]
}