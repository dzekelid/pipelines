{
  "info": {
    "name": "Bitbucket Add Repositories Username Repo Slug Pipelines Pipeline Uu Stoppipeline",
    "_postman_id": "e6ce90e2-26de-434f-a37b-861f55c33774",
    "description": "Signal the stop of a pipeline and all of its steps that not have completed yet.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "repositories",
      "item": [
        {
          "id": "5586e661-f42c-43d3-8aaf-055fbc115524",
          "name": "postRepositoriesUsernameRepoSlugPipelinesPipelineUuStoppipeline",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.bitbucket.org",
              "path": [
                "2.0",
                "repositories/:username/:repo_slug/pipelines/:pipeline_uuid/stopPipeline"
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
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Signal the stop of a pipeline and all of its steps that not have completed yet"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8e0c3b91-0024-4cbc-ace2-ae12dd5a48b4"
            }
          ]
        }
      ]
    }
  ]
}