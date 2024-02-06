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
`content/pages`. Each subdirectory of `content/pages` becomes a section in the
menu, `_index.md` is the content of the section, and other Markdown files in
the subdirectory become pages nested under that section.

Set `weight` in the Markdown headers to change the ordering of pages in the
menu.

# Templates

To use templates within Markdown files you must use shortcodes. Create a
shortcode by creating an HTML file in `layouts/shortcodes`. If you create
`layouts/shortcodes/template.html` then you would use the shortcode in a
Markdown file with `{{< template >}}`.

Use `{{< footer >}}` at the bottom of a Markdown file to use the common footer.

# Resources

[Hugo docs](https://gohugo.io/documentation/)

[Hugo Book Theme](https://github.com/alex-shpak/hugo-book)
