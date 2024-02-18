This is a base Node JS Project template, which has been prepared ny keeping some of the most important code principle and project management recommendation.

`src` -> all source code regarding the project will reside inside this folder, this will not include any tests.

Lets have a look inside the `src` folder

 - `config` -> In this folder anything and everything regarding any configuration or setup of a library or module will be done. For example: setting up `dotenv` so that we can use the environment variable any a cleaner fashion, this is done in `server-config.js`. One more example can be to setup a logging library which can be useful to make meaningful logs.

 - `routes` -> In the rotes folder, we register a routes and corresponding middleware and controllers to it.
