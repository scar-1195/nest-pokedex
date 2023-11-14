<p align="center">
   <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="200" alt="Nest Logo" /></a>
</p>

# Run App (dev)

1. Clone the repository
2. Run

```
yarn install
```

3. Have Nest CLI installed

```
npm i -g @nestjs/cli
```

4. Raise the database

```
docker-compose up -d
```

5. Clone the file `.env.template` and rename the copy to `.env`

6. Fill the environment variables defined in the `.env`

7. Run the application in dev:

```
yarn start:dev
```

8. Rebuild the database with the seed

```
http://localhost:3000/api/v2/seed
```

## Stack used

- MongoDB
- Nest

# ProductionBuild

1. Create the file `.env.prod`
2. Fill prod environment variables
3. Create the new image

```
docker-compose -f docker-compose.prod.yaml --env-file .env.prod up --build
```
