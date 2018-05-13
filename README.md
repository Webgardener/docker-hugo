# Webgardener.fr

Website powered by a containerized Hugo application (https://gohugo.io).

## Environment Variables

* `HUGO_THEME`
* `HUGO_WATCH` (set to any value to enable watching)
* `HUGO_DESTINATION` (Path where hugo will render the site. By default `/output`)
* `HUGO_REFRESH_TIME` (in seconds, only applies if not watching, if not set, the container will build once and exit)
* `HUGO_BASEURL`

## Template

The beautiful [Transcend template](https://colorlib.com/wp/template/transcend) from Colorlib was adapted for Hugo.
