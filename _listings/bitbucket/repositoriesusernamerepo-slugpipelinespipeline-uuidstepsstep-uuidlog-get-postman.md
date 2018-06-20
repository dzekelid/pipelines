{
  "info": {
    "name": "Bitbucket Get Repositories Username Repo Slug Pipelines Pipeline Uu Steps Step Uu Log",
    "_postman_id": "4461c718-aaf2-4736-8e55-6d924f03f159",
    "description": "Retrieve the log file for a given step of a pipeline.\n\nThis endpoint supports (and encourages!) the use of [HTTP Range requests](https://tools.ietf.org/html/rfc7233) to deal with potentially very large log files.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "repositories",
      "item": [
        {
          "id": "b398f0d9-74cb-4e10-be90-0b0184f4f616",
          "name": "getRepositoriesUsernameRepoSlugPipelinesPipelineUuStepsStepUuLog",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.bitbucket.org",
              "path": [
                "2.0",
                "repositories/:username/:repo_slug/pipelines/:pipeline_uuid/steps/:step_uuid/log"
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
            "description": "Retrieve the log file for a given step of a pipeline"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "93e10716-34bf-464e-90e0-3cdc470a301e"
            }
          ]
        }
      ]
    }
  ]
}