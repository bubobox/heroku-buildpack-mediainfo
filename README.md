# Heroku buildpack: Mediainfo
This is a [Heroku buildpack](http://devcenter.heroku.com/articles/buildpacks) for using [mediainfo](https://mediaarea.net/en/MediaInfo) in your project.
It doesn't do anything else, so you should use this as an extra buildpack on top of another buildpack. Heroku has build in support for using [multiple buildpacks](https://devcenter.heroku.com/articles/using-multiple-buildpacks-for-an-app). You can also use this [multi buildpack project](https://devcenter.heroku.com/articles/using-multiple-buildpacks-for-an-app) as main buildpack and configure your buildpacks via a `.buildpacks` file.

## Usage
This examples shows how you could add mediainfo to our existing app:

```
heroku buildpacks:add https://github.com/bubobox/heroku-buildpack-mediainfo -a <app>
```
