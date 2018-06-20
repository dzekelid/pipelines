{
  "info": {
    "name": "Bitbucket Get Repositories Username Repo Slug Pipelines Pipeline Uu",
    "_postman_id": "bc6c3a9b-b460-407c-829c-42efc5735c52",
    "description": "Get repositories username repo slug pipelines pipeline uu",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "repositories",
      "item": [
        {
          "id": "871591b0-df3b-4599-962f-dad95b7abf8b",
          "name": "getRepositoriesUsernameRepoSlugPipelinesPipelineUu",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.bitbucket.org",
              "path": [
                "2.0",
                "repositories/:username/:repo_slug/pipelines/:pipeline_uuid"
              ],
              "variable": [
                {
                  "id": "pipeline_uuid",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "repo_slug",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "username",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get repositories username repo slug pipelines pipeline uu"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b712ff7e-9b01-48be-9806-ba37e4cdbab1"
            }
          ]
        }
      ]
    }
  ]
}