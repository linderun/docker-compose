## Install

### 1. Clone the source code.

```shell
git clone https://github.com/linderun/docker-compose.git
```

### 2. Set the basic config

```shell
cd docker-compose && cp .env.example .env
```

Edit the `.env` file and set the config for the docker compose after you copy the `.env`.example file.

### 3. Build your app with Compose

```shell
docker-compose build
```

### 4. Run your app with Compose

```shell
docker-compose up -d
```

### 5. Experiment with some other commands

If you want to run your services in the background, you can pass the `-d` flag (for “detached” mode) to `docker-compose up` and use `docker-compose ps` to see what is currently running:

```shell
docker-compose ps
```

The `docker-compose run` command allows you to run one-off commands for your services. For example, to see what environment variables are available to the `nginx` service:

```shell
docker-compose run nginx env
```

If you started Compose with `docker-compose up -d`, stop your services once you’ve finished with them:

```shell
docker-compose stop
```

## Contributors

- [Darren Lin](http://github.com/linderun)

## License

The project is open-sourced software licensed under the [MIT license](http://opensource.org/licenses/MIT).

Web Site: [Darren Lin](http://www.linderun.com)
