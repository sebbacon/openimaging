## Deploying to Dokku

Follow "first time" instructions below, then deploys are handled by

```sh
git push dokku master
```

### First time

On the server:

```sh
dokku apps:create openimaging-web
dokku buildpacks:add openimaging-web https://github.com/heroku/heroku-buildpack-static
```

Locally:

```
git remote add dokku dokku@dokku.ebmdatalab.net:openimaging-web
git push dokku master
```
