Heroku Buildpack for Node.js and gulp.js
========================================

Usage
-----

- Set your Heroku app's buildpack URL to `heroku config:set BUILDPACK_URL=https://github.com/kehittamo/heroku-buildpack-nodejs-gulp-bower.git`
- Run `heroku config:set NPM_CONFIG_PRODUCTION=false` to allow the Heroku instance to install devDependencies stored in your package.json as [heroku recommends](https://devcenter.heroku.com/articles/nodejs-support#customizing-the-build-process).
- Run `heroku config:set NODE_ENV=production` to set your environment to `production` (or any other name)
- Add a Gulp task called `heroku:production` that builds your app
- Serve your app using Express or whatever

Credits
-------

Forked from [heroku-buildpack-nodejs](https://github.com/heroku/heroku-buildpack-nodejs).

Heavily based on [heroku-buildpack-nodejs-grunt](https://github.com/mbuchetics/heroku-buildpack-nodejs-grunt).
