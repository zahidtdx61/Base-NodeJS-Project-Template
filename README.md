This is a base Node JS Project template, which has been prepared ny keeping some of the most important code principle and project management recommendation.

`src` -> all source code regarding the project will reside inside this folder, this will not include any tests.

Lets have a look inside the `src` folder

-   `config` -> In this folder anything and everything regarding any configuration or setup of a library or module will be done. For example: setting up `dotenv` so that we can use the environment variable any a cleaner fashion, this is done in `server-config.js`. One more example can be to setup a logging library which can be useful to make meaningful logs.

-   `routes` -> In the rotes folder, we register a routes and corresponding middleware and controllers to it.

-   `middlewares` -> as middlewares they can process incoming request for validation and authentication.

-   `controllers` -> they are kind of the last middlewares as post them you call you business layer to execute the business logic. In controllers we just receive the incoming requests and data and then pass it to the business layer, and once business layer returns an output, we structure the API response in controllers and send the output.

-   `repositories` -> this folder contains all the logic using which we interact the DB by writing queries, all the raw queries or ORM queries will go here.

-   `services` -> contains the business logic and interacts with repositories for data from the database.

-   `utils` -> contains helper methods, error classes etc.

### Setup the project

-   download this template and open it any text editor.

-   go inside the root directory and run the following command:

```
npm install
```

-   In the root directory create a `.env` file and add the following env variables

```
PORT=<port number of your choice>
```

ex:

```
PORT=3000
```

-   go inside the `src` folder and execute the following command:

```
npx sequelize init
```

-   By executing the above command you will get migrations and seeders folder along with a config.json inside the config folder.

-   For setting up development environment, write the username and password of db and in dialect mention whatever db is being used for ex: mysql, mariadb etc

-   For setting up test or prod environment, make sure to replace the host with the hosted db url.

-   To run the server execute

```
npm start
```
