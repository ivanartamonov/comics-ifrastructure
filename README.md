# Comics Infrastucture

We have `backend` and `frontend` in separate repositories.
Current repo is infrustructure for launching backend and frontend together with Docker.

## How to use

You should clone this repo and after that

```
clone <backend repository> backend
clone <frontend repository> frontend

docker-compose up -d --build
```

Docker will build required containers and after that you can open backend & frontend websites with browser by the following adresses:

* Backend: http://localhost:8080
* Frontend http://localhost:8081

You can change some files in `backend`/`frontend` directoies and check that websites are changing too.

Have fun!