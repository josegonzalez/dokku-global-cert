# dokku-global-cert [![Build Status](https://travis-ci.org/josegonzalez/dokku-global-cert.svg?branch=master)](https://travis-ci.org/josegonzalez/dokku-global-cert)

Allow setting a global certificate for dokku applications.

## requirements

- dokku 0.5.0+
- docker 1.10.x

## installation

```shell
# on 0.5.x
dokku plugin:install https://github.com/josegonzalez/dokku-global-cert.git  global-cert
```

## usage

```shell
# first create the global certificate directory:
mkdir -p /var/lib/dokku/config/global-cert/

# now copy your cert and key into this directory
cp server.crt /var/lib/dokku/config/global-cert/server.crt
cp server.key /var/lib/dokku/config/global-cert/server.key

# and now all applications being deployed will have
# the global certificate automatically set
```
