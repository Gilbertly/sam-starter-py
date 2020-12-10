# sam-starter-py
## Setup
```sh
// activate pipenv
$ pipenv shell

// install dependencies
$ pipenv install && pipenv install --dev
```

## Deployment
```sh
// generate requirements.txt from pipenv
$ pipenv lock --requirements > ./requirements.txt
$ cp ./requirements ./src/functions/requirements.txt

// validate and build project
$ sam validate && sam build

// deploy to dev env
$ sam deploy --config-env dev

// deploy to prod env
$ sam deploy --config-env prod
```