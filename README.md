# tableau-rest-tutorial
Fully automated Postman collection for the Tableau Server REST API tutorial

1. To get started, import the collection via Postman's Github integration or clone the repository and import it as a local file.
2. Create a Postman environment called `Tableau REST API`.
3. Add three environment variables used when authenticating into Tableau Server: `username`, `password`, `content-url` as defined in the [API Docs](https://help.tableau.com/current/api/rest_api/en-us/REST/rest_api_concepts_auth.htm).

>The collection has a Sign In request that is scripted to use the environment variables from step #3. Additionally, there is a collection level script that performs the same task (see Pre-Request Script for the Collection) for every single request. As a result any request made with the collection will first authenticate and update the collection variables `site-id` and `api-key`. Manual authentication is no longer required.

4. Make any request or perform the Sign In request to update the `site-id` and `api-key` collection variables.
