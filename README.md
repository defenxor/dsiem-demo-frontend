# Dsiem Demo — Frontend

Elastic UI framework app that combines all Dsiem features and integrations in a single interface.

## Usage

Full usage requires a [`docker-compose.yml`](https://github.com/defenxor/dsiem/blob/master/demo/docker/docker-compose.yml) that defines all the other components: ELK, filebeat, APM, ossec, suricata, dsiem, wise, nesd, and a web server that is vulnerable to Shellshock exploit.

But for development purposes, just:

```shell
$ cd web && yarn install && yarn start
```

The web app should be available at `http://localhost:3000`

## Building

Requirements:

- NPM
- Docker
- Yarn (`npm install --global yarn`)

Building just the web app:

```shell
$ cd web && yarn install && yarn build
```

Building the docker image:

```shell
$ ./build.sh
```
