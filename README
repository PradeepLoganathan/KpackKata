Companion project for blog post at https://pradeepl.com/kpack
A sample project to demonstrate setting up Kpack with all its necessary components such as 
 - ClusterBuilder
 - ClusterStack
 - ClusterSource
 - Image

## Create a Docker Hub Access Token

1. Log in to your Docker Hub account.
2. Navigate to Settings.
3. Select Security.
4. Click on New Access Token.
5. Give the token a name (e.g., "kpack-token") and select the appropriate permissions.
6. Copy the generated token (you won’t be able to see it again).

Update the registry-secret.yaml file with the base64 encoded value of your docker config json. The docker config json looks like this 

```json
{
  "auths": {
    "https://index.docker.io/v1/": {
      "username": "<YOUR_DOCKERHUB_USERNAME>",
      "password": "<DOCKERHUB_ACCESS_TOKEN>",
      "email": "<YOUR_EMAIL>"
    }
  }
}
```

Replace <YOUR_DOCKERHUB_USERNAME>, <DOCKERHUB_ACCESS_TOKEN>, and <YOUR_EMAIL> with your information. After creating the JSON, base64 encode it and place it in the YAML file.

To base64 encode, you can use ```echo -n '<JSON_CONTENT>' | base64
```