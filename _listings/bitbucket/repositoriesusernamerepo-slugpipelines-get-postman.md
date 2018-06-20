{
  "info": {
    "name": "Bitbucket Get Repositories Username Repo Slug Pipelines",
    "_postman_id": "56fe6e43-8fa8-4b3f-9aaa-b2b721d6b53a",
    "description": "Get repositories username repo slug pipelines",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "repositories",
      "item": [
        {
          "id": "e50f150e-bba0-4113-ab5e-9eadf785963f",
          "name": "getRepositoriesUsernameRepoSlugPipelines",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.bitbucket.org",
              "path": [
                "2.0",
                "repositories/:username/:repo_slug/pipelines/"
              ],
              "variable": [
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
            "description": "Get repositories username repo slug pipelines"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "52b56777-4097-44c1-8843-43a32d48f9ab"
            }
          ]
        }
      ]
    }
  ]
}