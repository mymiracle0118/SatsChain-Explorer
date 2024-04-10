<h1 align="center">
    <strong>Satschain frontend</strong>
</h1>
<p align="center">
    <strong>Frontend application for sats blockchain explorer</strong>
</p>



## Requirements

You need to use node v20.11.0
```
nvm install v20.11.0
nvm alias default v20.11.0
nvm use

node --version
```

You need to install yarn

## Clone the repo

You can clone the repo
```
git clone git@github.com:satschaintech/etherscanindexer.git && cd etherscanindexer
```

## Setting env vars
You need to copy `.env.development` to `.env.development.local`
```
cp .env.development .env.development.local
```

You need to set env vars
```
...
NEXT_PUBLIC_APP_PROTOCOL=http                   # your explorer 
NEXT_PUBLIC_APP_HOST=localhost                  # your explorer ( I think you should use http://localhost for testing for the first time )
NEXT_PUBLIC_APP_PORT=4000                       # your explorer port

NEXT_PUBLIC_AUTH_URL=http://localhost:4000      # your explorer host
# api configuration
NEXT_PUBLIC_API_PROTOCOL=http                   # API config
NEXT_PUBLIC_API_HOST=localhost
NEXT_PUBLIC_API_PORT=8300                       # API port, it must be same as server's EXPLORER_SERVER_PORT
NEXT_PUBLIC_API_BASE_PATH=/
...

```

## Running the app

You can run the app by using following command
```
yarn dev
```

You can open link, for example `http://localhost:4000`

You can check integration in `blocks` page