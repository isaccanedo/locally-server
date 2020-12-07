# locally-server

[![Build Status][travis-image]][travis-url]
[![Dependency Status][dependency-image]][dependency-url]
[![devDependency Status][devdependency-image]][devdependency-url]
[![Code Style][style-image]][style-url]

> A JSON file RESTful API with authorization based on [json-server](https://github.com/typicode/json-server) for [zce/weapp-locally](https://github.com/zce/weapp-locally) & [zce/quickapp-locally](https://github.com/zce/quickapp-locally)

## Usage

```sh
# clone repo
$ git clone https://github.com/zce/locally-server.git <my-api-server>

# change directory
$ cd <my-api-server>

# install dependencies
$ yarn # or npm install
```

modify [database.json](database.json) file

```sh
# serve with hot reload at http://localhost:3000
$ yarn dev
```

## JSON Server Resources Endpoints

- Slides: `/slides/:id?`
- Categories: `/categories/:id?`
- Shops: `/shops/:id?`

To access and modify resources, you can use any HTTP method: `GET` `POST` `PUT` `PATCH` `DELETE` `OPTIONS`

## Backdoor Endpoints

### GET `/backdoor/delay`

add a delay of 1000ms for each endpoint

```sh
$ curl http://localhost:3000/backdoor/delay
```
