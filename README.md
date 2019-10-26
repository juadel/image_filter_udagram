
## PERSONAL NOTES:
-API URL :image-filter-udagram-dev.ca-central-1.elasticbeanstalk.com , endpoint "/filteredimage"
- Tried to catch errors using try/catch but I am having problems to control UNHANDLE PROMISE REJECTIONS. That happend when the URL provide do not link to a valid IMAGE.
- Also tried to add an endpoint in the feed.router.ts restapi, so only Authenticated user were able to filter the image, however, I was not able to handle the response. You can check what I tried in : https://github.com/juadel/udacity-c2-restApi


# Udagram Image Filtering Microservice
## Tasks

### Setup Node Environment

You'll need to create a new node server. Open a new terminal within the project directory and run:

1. Initialize a new project: `npm i`
2. run the development server with `npm run dev`

### Create a new endpoint in the server.ts file

The starter code has a task for you to complete an endpoint in `./src/server.ts` which uses query parameter to download an image from a public URL, filter the image, and return the result.

We've included a few helper functions to handle some of these concepts and we're importing it for you at the top of the `./src/server.ts`  file.

```typescript
import {filterImageFromURL, deleteLocalFiles} from './util/util';
```

### Deploying your system

Follow the process described in the course to `eb init` a new application and `eb create` a new environment to deploy your image-filter service! Don't forget you can use `eb deploy` to push changes.

## Stand Out (Optional)

### Refactor the course RESTapi

If you're feeling up to it, refactor the course RESTapi to make a request to your newly provisioned image server.

### Authentication

Prevent requests without valid authentication headers.
> !!NOTE if you choose to submit this, make sure to add the token to the postman collection and export the postman collection file to your submission so we can review!

### Custom Domain Name

Add your own domain name and have it point to the running services (try adding a subdomain name to point to the processing server)
> !NOTE: Domain names are not included in AWS’ free tier and will incur a cost.
