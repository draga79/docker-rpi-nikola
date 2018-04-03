![License MIT](https://img.shields.io/badge/license-MIT-blue.svg) [![Docker Automated build](https://img.shields.io/docker/automated/dragas/rpi-nikola.svg)](https://hub.docker.com/r/dragas/rpi-nikola) [![](https://img.shields.io/docker/stars/dragas/rpi-nikola.svg)](https://hub.docker.com/r/dragas/rpi-nikola) [![](https://img.shields.io/docker/pulls/dragas/rpi-nikola.svg)](https://hub.docker.com/r/dragas/rpi-nikola)

# Nikola

This [Docker](https://www.docker.com) image contains a complete [Nikola](https://getnikola.com/) installation, ready for use. 

## About Nikola

Nikola is a static website and blog generator. It supports many input formats. It is fast and reliable. Have a [look here](https://getnikola.com/).

## Quickstart

This section assumes you want to get started quickly, the following sections explain the
steps in more detail. So let's start.

The container has been created with workdir set on /nikola, so any command given should be given keeping in mind this setup.

To initialize a new website, use the following command:

```bash
$ docker run --rm -ti -v /yourpath:/nikola dragas/rpi-nikola nikola init
```

Running this command for the first time will download the image automatically. Nikola will ask some questions and prepare its path. The container will then terminate and delete as all Nikola data will be stored in */yourpath*

For Nikola usage, please refer to its original documentation: [Nikola Handbook](https://getnikola.com/handbook.html)
