# Static site Docker

Simple steps are the following:

- Clone the repository

```git clone https://github.com/zoparga/static-site-docker.git```

- Copy .env.example file to .env

```cp .env.example .env```

- Edit .env file, change app name, environment, and the most important -> port numbers if needed!

```
NGINX_80=DESIRED_PORT_NUMBER_INSTEAD_OF_80
NGINX_443=DESIRED_PORT_NUMBER_INSTEAD_OF_443
```

- Run container

``` docker-compose up -d ```

- Fill the **www** folder with files what you want to host.
