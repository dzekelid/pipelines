{
  "info": {
    "name": "AWS Code Pipeline API Get Pipeline State",
    "_postman_id": "a3030c5e-0fde-40f7-b555-3c1873ae7bac",
    "description": "Returns information about the state of a pipeline, including the stages and\n            actions.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Pipeline",
      "item": [
        {
          "id": "1a117d60-400e-4318-b21a-225cecaed396",
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
              "id": "29c80a21-fbea-4d96-92e4-782a9b1af662"
            }
          ]
        }
      ]
    }
  ]
}