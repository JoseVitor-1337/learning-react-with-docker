# React with Docker

### How to create a react application and deploy with docker

<br />

## Technologies used

### Frontend

- [React.js](https://pt-br.reactjs.org/)

### Infrastructure

- [Docker](https://docs.docker.com/engine/install/ubuntu/)

<br />

## Required installation

> Need have **docker** installed [Install Docker](https://docs.docker.com/engine/install/ubuntu/)

> Need have **npm** installed [Install NPM](https://nodejs.org/en/)

> Need have **git** installed [Install git](https://git-scm.com/downloads)

<br />

## Docker Commands

Build a image docker and start the container in develoment mode

```
  docker-compose -f docker-compose.dev.yml up -d --build
```

Build a image docker and start the container in production mode

```
  docker-compose -f docker-compose.prod.yml up -d --build
```

- command **up** will execute the docker-compose files

- flag **-f** specifies path to docker-compose file

- flag **-d** make the container run in background so it doesn't stay in the terminal

- flag **-build** if there is a change in the specified root files, it will rerun the build

## Usage

Install all dependencies

```
  npm install
```

To display docker-compose to build a image **react-app-dev** and run the container:

```
  npm docker:dev
```

To display docker-compose to build a image **react-app-prod** and run the container:

```
  npm docker:prod
```

Dev server will be running on [http://localhost:3000](http://localhost:3000)

Production server will be running on [http://localhost:8080](http://localhost:8080)
