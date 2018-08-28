{
  "info": {
    "name": "Bitbucket Get Repositories Username Repo Slug Pipelines Pipeline Uu Steps",
    "_postman_id": "751f0918-0a23-47d0-a0cb-da66fc7e621f",
    "description": "Get repositories username repo slug pipelines pipeline uu steps",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "repositories",
      "item": [
        {
          "id": "5c75537a-9ed4-40db-80eb-aad63314f7c8",
          "name": "getRepositoriesUsernameRepoSlugPipelinesPipelineUuSteps",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.bitbucket.org",
              "path": [
                "2.0",
                "repositories/:username/:repo_slug/pipelines/:pipeline_uuid/steps/"
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
            "description": "Get repositories username repo slug pipelines pipeline uu steps"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1891f6bc-6676-4521-b959-a4160a36e8e8"
            }
          ]
        }
      ]
    }
  ]
}