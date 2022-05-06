# Comics Infrastucture

We have `backend` and `frontend` in separate repositories.
Current repo is infrustructure for launching backend and frontend together with Docker.

## How to use

You should clone this repo and enter to the directory

```
git clone https://github.com/ivanartamonov/comics-ifrastructure.git comics
cd comics
```

Clone git sub-modules
```
git submodule update --init
```

Build docker container
```
docker-compose up --build -d
```

Install backend dependecies
```
docker-compose exec comics_php composer install
```

Now, you can open backend website by http://localhost:8080

Enter to `frontend` directory and start working with frontend
```
cd frontend
yarn install
yarn start
```

Now, you can open frontend app by http://localhost:3000

Tip: you can enter to `backend` or `frontend` directory and switch branch separately in frontend and backend applications.

Have fun!