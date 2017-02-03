# Heroku buildpack: Mediainfo
This is a [Heroku buildpack](http://devcenter.heroku.com/articles/buildpacks) for using [mediainfo](https://mediaarea.net/en/MediaInfo) in your project.
It doesn't do anything else, so you should use this as an extra buildpack on top of another buildpack. Heroku has build in support for using [multiple buildpacks](https://devcenter.heroku.com/articles/using-multiple-buildpacks-for-an-app). You can also use this [multi buildpack project](https://devcenter.heroku.com/articles/using-multiple-buildpacks-for-an-app) as main buildpack and configure your buildpacks via a `.buildpacks` file.

## Usage
This examples shows how you could add mediainfo to our existing app:

```
heroku buildpacks:add https://github.com/bubobox/heroku-buildpack-mediainfo -a <app>
```

The binary location will be added to your PATH environment variable so after adding the buildpack and pushing a new commit `mediainfo` should be available to any shell command.

## Binary information

The binaries for this buildpack are compiled using the following compile flags

```
--with-libcurl
```

## Contribute

We really appreciate any contribution you would like to make, so don't
hesitate to report issues or submit pull requests.

## About us

If you would like to know more about us, be sure to have a look at [our website](https://www.ambassify.com), or our Twitter accounts [Ambassify](https://twitter.com/Ambassify), [Sitebase](https://twitter.com/Sitebase), [JorgenEvens](https://twitter.com/JorgenEvens)
