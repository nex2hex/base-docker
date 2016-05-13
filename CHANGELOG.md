# Changelog

## 3.10 (2016-05-13)

* freeze pip to 8.1.1 also in default virtualenv


## 3.9 (2016-05-13)

* freeze pip to 8.1.1 because of issues with pip-compile


## 3.8 (2016-05-13)

* Update forego install source


## 3.7 (2016-05-09)

* set LC_ALL and LANG env vars to correctly support python3
* install pipsi and pip-tools with python3 for the python3 version
  (fixes problems with not finding wheels)


## 3.6 (2016-05-09)

* re-build to pick up latest python base image changes (e.g pip 8.1.1)
* remove --prompt from virtualenv creation


## 3.5 (2016-04-25)

* re-build to pick up latest python base image changes


## 3.4 (2016-03-07)

* build two images: python 2 and python 3
  (python 3 versions are tagged as py3-x.x)
* use tini as PID1 (kills zombies)


## 3.0 (2015-08-28)

* switch to debian as base (using the official python:2.7.10 docker image)
* a default virtualenv with --no-site-packages (at /virtualenv) that is activated
* pipsi
* no more globally installed python packages (mercurial, bzr are now installed with pipsi)
* pip-tools
* node/npm not installed anymore


## 2.6 (2015-07-14)

* newer ubuntu packages
* less layers
* run-forest-run command


## 2.5 (2015-03-03)

* add forego, a foreman clone in go


## 2.4 (2015-02-19)

* extra packages also installed on python:latest
* python encoding fixes


## 2.3 (2015-03-08)

* libffi-dev for pyOpenSSL/cryptography
* libpcre
* supervisor
* unzip
* wget
* node/npm


## 2.2 (2014-11-18)

* Procfile based startup


## 2.1 (2014-08-27)

* adds libncurses5-dev


## 2.0 (2014-08-06)

* ubuntu 14.04
* libgeoip
* removed java