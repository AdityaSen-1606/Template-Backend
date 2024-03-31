This is a base node JS project template, which anyone can use as it has been prepared by keeping some of the most important code principles & project management recommendation. Feel fee to change anything.

`src` -> Inside the src folder all the actual source code regarding the project will reside, this will not include any kind of tests.

Lets take a look inside the `src` folder

- `config` -> In this folder anything and everything regarding any configurations or setup of library or module will be done. For example: setting up `dotenv` so that we can use the environment variables anywhere in a cleaner fashion, this is done in the `server-config.js`. One more example can be to setup you logging library that can help you to prepare meaningful logs, so configuration for this library should also be done here.

- `routes` -> In the routes folder, we register a route and the corresponding middleware and controlling to it.

- `middlewares` -> they are just going to intercept the incoming requests where we can write our validators, authenticators etc.

- `controllers` -> they are kind of last middleware as post then you call you business layer to execute the business logic. In controller we just receive the incoming requests & data and then pass it to the business layer, and once business layer return an output, we structure the API response in controllers and send the output.

-`repositories` -> this folder contains all logic using which we can interact the DB by writing queries, all the raw queries or ORM queries will go here.

- `services` -> contains business logic and interact with repositories for data from DB

-`utils` -> contains helper methods, error classes etc.

### Setup the project

- Download this template from github and open it in your favourite text editor.
- In the root directory create a `.env` file and add the following env variables
