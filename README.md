# Dockerize Symfony

With this project, you can quickly containerize a Symfony project with KnpSnappyBundle support for PDF generation.

Contents:

- [Requirements](#requirements)
- [Configuration](#configuration)
- [Usage](#usage)
- [Installed](#installed)

## Requirements

Make sure you have the latest versions of `Docker` and `Docker Compose` installed on your machine.

## Configuration

1. Copy the files from this repository into the folder with existing Symfony project.

2. Copy variables from `.env.example` to `.env` file and adapt them to your needs.

3. Place a dump of your MySQL database in the ./docker/db folder. It will be imported automatically.

## Usage

Build and run containers (in daemon mode):
```
docker-compose up -d
```

Open the Symfony project at the address (if you haven't changed the default port):
```
https://127.0.0.1:701
```

Stop and remove the containers:
```
docker-compose down
```

## Installed

1. PHP 8.1
2. MySQL 8
3. Xdebug
4. Wkhtmltopdf
5. Composer
6. Node 18
7. SSL self-signed certificate
8. Adminer and phpMyAdmin database management tools
9. Git
10. Cron job for messenger
