[![Docker Stars](https://img.shields.io/docker/stars/frolvlad/alpine-miniconda2.svg?style=flat-square)](https://hub.docker.com/r/frolvlad/alpine-miniconda2/)
[![Docker Pulls](https://img.shields.io/docker/pulls/frolvlad/alpine-miniconda2.svg?style=flat-square)](https://hub.docker.com/r/frolvlad/alpine-miniconda2/)


Miniconda Python 2.7 Docker image
=================================

This image is based on Alpine Linux image, which is only a 5MB image, and contains
[Python 2.7](https://www.python.org/) packaged by Continuum with Conda package manager.

Total size of this image is only:

[![](https://badge.imagelayers.io/frolvlad/alpine-miniconda2:latest.svg)](https://imagelayers.io/?images=frolvlad/alpine-miniconda2:latest 'Get your own badge on imagelayers.io')

NOTE: Conda repositories contain only Glibc linked packaged binaries for Linux,
so we have to use
[glibc workaround](https://github.com/gliderlabs/docker-alpine/issues/11) on
Alpine.


Usage Example
-------------

```bash
$ docker run --rm frolvlad/alpine-miniconda2 python -c 'print u"Hello World"'
```

Once you have run this command you will get printed 'Hello World' from Python!

NOTE: `conda` and `pip` are also available in this image.
