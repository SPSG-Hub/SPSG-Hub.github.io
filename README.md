# Local Testing

Install Hugo: [https://gohugo.io/installation/](https://gohugo.io/installation/)

Clone this repoository and use the `--recurse-submodules` option to pull in the
theme when cloning.

In the repo directory run the following to start a local server:

```
hugo server --minify --theme hugo-book
```

This should print a URL to visit to see the local version of the site. Editing
files will restart the server automatically.

# Content Structure

The main page is `content/_index.md`. The menu on the left is built from
`content/pages` (the README needs to be expanded here to describe how to have
nested items on the menu).

# Resources

[Hugo docs](https://gohugo.io/documentation/)

[Hugo Book Theme](https://github.com/alex-shpak/hugo-book)
