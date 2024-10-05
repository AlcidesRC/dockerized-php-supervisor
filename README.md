[![Continuous Integration](https://github.com/AlcidesRC/dockerized-php-supervisor/actions/workflows/ci.yml/badge.svg)](https://github.com/AlcidesRC/dockerized-php-supervisor/actions/workflows/ci.yml)

# Dockerized PHP - Supervisor


> A _dockerized_ environment based on Supervisor + PHP-FPM running on a Linux Alpine container. 


[TOC]

------



## Summary

This repository contains a _dockerized_ environment for building PHP applications based on **php:8.3.12-fpm-alpine** with Supervisor support.

### Highlights

- Unified environment to build <abbr title="Command Line Interface">CLI</abbr>, <u>web applications</u> and/or <u>micro-services</u> based on **PHP8**.
- Allows you to create an optimized **development environment** Docker image
- Allows you to create an optimized **production-ready** Docker image
-  Using **built-in PHP webserver**.
-  PHP-FPM and built-in webserver are managed by Supervisor.



------



## Requirements

To use this repository you need:

- [Docker](https://www.docker.com/) - An open source containerization platform.
- [Git](https://git-scm.com/) - The free and open source distributed version control system.
- [Make](https://www.gnu.org/software/make/) - A command to automate the build/manage process.
- [jq](https://jqlang.github.io/jq/download/) - A lightweight and flexible command-line JSON processor.



------



## Built with

| Type           | Component                                                | Description                                                  |
| -------------- | -------------------------------------------------------- | ------------------------------------------------------------ |
| Infrastructure | [Docker](https://www.docker.com/)                        | Containerization platform                                    |
| Service        | [Supervisor](http://supervisord.org/)                    | Supervisor is a client/server system that allows its users to control a number of processes on UNIX-like operating systems. |
| Service        | [PHP-FPM](https://www.php.net/manual/en/install.fpm.php) | PHP with FastCGI Process Manager                             |
| Miscelaneous   | [Bash](https://www.gnu.org/software/bash/)               | Allows to create an interactive shell within containerized service |
| Miscelaneous   | [Make](https://www.gnu.org/software/make/)               | Allows to execute commands defined on a _Makefile_           |
| Miscelaneous   | [jq](https://jqlang.github.io/jq/download/)              | Allows to beautify the Docker inspections in JSON format     |



------



## Development Environment



> [!IMPORTANT]
>
> This development environment is based on [Dockerized PHP](https://github.com/alcidesrc/dockerized-php), a framework agnostic *dockerized* environment to create and deploy PHP applications.
>
> Please take a look to the [README.md](https://github.com/alcidesrc/dockerized-php/blob/main/README.md) file to know how to familiarize with it and get up and running.



> [!IMPORTANT]
>
> Default application is based on [PHP Skeleton](https://github.com/alcidesrc/php-skeleton), a minimalistic boilerplate to create PHP applications from scratch.
>
> Please take a look to the [README.md](https://github.com/alcidesrc/php-skeleton/blob/main/README.md) file to know how to familiarize with it and get up and running.



------



## Getting Started

Just clone the repository into your preferred path:

```bash
$ mkdir -p ~/path/to/my-new-project && cd ~/path/to/my-new-project
$ git clone git@github.com:alcidesrc/dockerized-php-supervisor.git .
```

### In short

```bash
$ make init
```

### TL;DR

#### Building the container

```bash
$ make build
```

#### Starting the container service

```bash
$ make up
```

#### Accessing to Supervisor Status web panel

```bash
$ make open-supervisor
```

#### Accessing to web application

```bash
$ make open-website
```

#### Stopping the container service

```bash
$ make down
```



------




## Security Vulnerabilities

Please review our security policy on how to report security vulnerabilities:

**PLEASE DON'T DISCLOSE SECURITY-RELATED ISSUES PUBLICLY**

### Supported Versions

Only the latest major version receives security fixes.

### Reporting a Vulnerability

If you discover a security vulnerability within this project, please [open an issue here](https://github.com/alcidesrc/dockerized-php-supervisor/issues). All security vulnerabilities will be promptly addressed.



------



## License

The MIT License (MIT). Please see [LICENSE](./LICENSE) file for more information.
