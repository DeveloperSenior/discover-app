
# Electiva-II
# Team
- Discover Team
# Team members
- [Andres Escobar](https://github.com/DeveloperSenior)
# Technology in which it was developed
- NodeJS v18.19.1
# Project's name
`Discover App` It is a Back and Front application, which seeks to centralize products, launch them to a community and they can be reviewed and rated. It is also a Repository for the NodeJs learning space focused on Back-end, good development practices and design patterns.
# Back-End Project Structure
The project was developed for the back-end with NodeJS v18.19.1, using the following support libraries:

1. `express` for the creation of the container
Rest API server and usage
2. `nodemon` tool that helps develop Node.js based applications by automatically restarting the node application when changes are detected in the files in the directory.
3. `rxjs` Library of reactive extensions for JavaScript
4. `fluent-json-schema` JSON Schema Generator
5. `ajv` JSON structure validator based on javascript object schemas (JSON).
6. `swagger-jsdoc`, `swagger-model-validator`, `swagger-ui-express` This module allows you to serve API documents automatically generated by swagger-ui from Express, based on a swagger spec with `swagger-jsdoc`. The result is live documentation for the API hosted from the API server through a route.
7. `mongoose` as ODM to persist JSON documents in MongoDB and`mongoose-paginate-v2` to perform paginated queries to MongoDB.
8. `jsonwebtoken` to authenticate and authorize each transaction in the API exposed by `express`.
9. `bcrypt` to encrypt and validate passwords that are stored in MongoDB

```
discover-app-api
  L src
    L controllers
    L db
        L conf
           L config.js
    L middleware
         L AuthMiddleware.js
    L models
       L dto
       L exception
       L schema
    L routes
       L config
          L SuscriptionRoutesAppConf.js
          L SwaggerRouteConf.js
    L services
    L utilities
        L Base64Util.js
        L Constants.js
        L Utilities.js
    L validator
  L test
     L controllers
     L db
     L middleware
     L models
     L routes
     L services
     L utilities
     L validators
  L discover-app-api.postman_collection
  L package.json
  L .env
  L app.js
  L server.js
  L jest.config.js
discover-app-front
  L src
L .gitignore
L README.md
``` 

# How to run the project
1. **Clone the Repository:**
```bash
git clone
https://github.com/DeveloperSenior/DiscoverTeam-ProductHunt-Electiva2.git
```
2. **Install node modules:**
```bash
cd discover-app-api
npm install
```
3. **Run unit tests with JEST:**
```bash
npm run test
```
*NOTE:* To view the coverage report open the file`./coverage/index.html`

4. **Run the local application:**

**NOTE:** Before running the server, review the file `.env-example` and turn it into `.env` so that the server takes the initial configuration parameters. 
```bash
npm run runDev
```
5. Open in browser http://localhost:3000/api/v1/version If you answer a `JSON` so:
```json
{"version": "1.0"}
```
It means that our server is up.

6. **View Documentation :**
The API documentation is in the url http://localhost:3000/api/v1/api-docs/

6. **Postman collection :**
In the Postman tool import the file `discover-app-api.postman_collection` which is at the root of the project.


# Front-End Project Structure

The project was developed for the front-end with Angular v17.3.1, using the following support libraries:

1. `mdb-angular-ui-kit` s a library that greatly extends the capabilities of regular Bootstrap.
2. `minidenticons` Generate identicons (pixelated avatars) on the client from usernames instead of fetching images from a server. Much faster, saves bandwidth and GDPR compliant.
3. `rxjs` Library of reactive extensions for Angular TypeScript and JavaScript
4. `@angular/material` The Angular team builds and maintains both common UI components and tools to help you build your own custom components
6. `@sweetalert2` A beautiful, responsive, customizable, accessible (WAI-ARIA) replacement for JavaScript's popup boxes. Zero dependencies.

# How to run the project
1. **Clone the Repository:**
```bash
git clone
https://github.com/DeveloperSenior/DiscoverTeam-ProductHunt-Electiva2.git
```
2. **Install node modules:**
```bash
cd discover-app-front
npm install
```

3. **Run the local application:**


```bash
npm start

```

5. Open in browser http://localhost:4200/ show home page, It means that our app is up.