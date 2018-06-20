{
  "info": {
    "name": "Bitbucket Get Repositories Username Repo Slug Pipelines Pipeline Uu Steps Step Uu",
    "_postman_id": "471cdd04-4826-4a1b-9f9e-b0d286adf66e",
    "description": "Get repositories username repo slug pipelines pipeline uu steps step uu",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "repositories",
      "item": [
        {
          "id": "8134febd-d631-48ca-9b1c-db7f2a74cee9",
          "name": "getRepositoriesUsernameRepoSlugPipelinesPipelineUuStepsStepUu",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.bitbucket.org",
              "path": [
                "2.0",
                "repositories/:username/:repo_slug/pipelines/:pipeline_uuid/steps/:step_uuid"
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
                  "id": "step_uuid",
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
            "description": "Get repositories username repo slug pipelines pipeline uu steps step uu"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "65e8e1be-28a1-45dc-8fda-07acb26c942d"
            }
          ]
        }
      ]
    }
  ]
}