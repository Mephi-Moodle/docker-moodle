docker-moodle
=============

A Dockerfile that installs the latest Moodle, Apache, PHP, MySQL and SSH

## Installation

```
git clone https://github.com/sergiogomez/docker-moodle.git
cd docker-moodle
docker build -t moodle .
```

## Usage

To spawn a new instance of Moodle:

```
docker run --name moodle1 -e VIRTUAL_HOST=moodle.test.ru -v /path/to/moodle:/var/www/html -d -t -p 3000:80 -p 3500:22 moodle
```

You can visit the following URL in a browser to get started:

```
http://127.0.0.1:3000/
```

Thanks to [eugeneware](https://github.com/eugeneware) and [ricardoamaro](https://github.com/ricardoamaro) for their Dockerfiles.