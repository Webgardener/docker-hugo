# Webgardener.fr

Website powered by a containerized Hugo application (https://gohugo.io).

## Environment Variables

* `HUGO_THEME`
* `HUGO_WATCH` (set to any value to enable watching)
* `HUGO_DESTINATION` (Path where hugo will render the site. By default `/output`)
* `HUGO_REFRESH_TIME` (in seconds, only applies if not watching, if not set, the container will build once and exit)
* `HUGO_BASEURL`

Create env.list file with values:

```
HUGO_THEME=simple-a
HUGO_WATCH=1
HUGO_REFRESH_TIME=360
HUGO_BASEURL=http://baseurl
```

## RUN
```
docker run --name "my-hugo" --publish-all   -p 32000:1313     --volume $(pwd)/src:/src        --volume /tmp/hugo-build-output:/output        --env-file env.list jojomi/hugo
```

## Template

The beautiful [Transcend template](https://colorlib.com/wp/template/transcend) from Colorlib was adapted for Hugo.
