
### Using Locally with Jekyll

First, install [Ruby](https://www.ruby-lang.org/en/) and [Jekyll](https://jekyllrb.com/). The install instructions can be found here: <https://jekyllrb.com/docs/installation/#guides>

```bash
bundle install
bundle add webrick
bundle exec jekyll server
```
View the live page using `localhost`:
<http://localhost:4000>. You can get the HTML files in `_site` folder.


### Edit included files

There are two markdown files included in `index.md`. They are `_includes/publications.md` and `_includes/service.md`, respectively. These two files also support **Markdown** and **HTML** syntax. If you don't hope to include these two files, you may remove the following lines in `index.md`:

If you hope to edit the publication list without changing the format, you may edit `_data/publications.yml`:


### Stylesheet

If you'd like to add your own custom styles, you may edit `_sass/minimal-light.scss`.

### Layouts

If you'd like to change the theme's HTML layout, you may edit `_layout/homepage.html`.

## License

This work is licensed under a [Creative Commons Zero v1.0 Universal](https://github.com/yaoyao-liu/minimal-light/blob/master/LICENSE) License.

## Acknowledgements

Our project uses the source code from the following repositories:

* [pages-themes/minimal](https://github.com/pages-themes/minimal)

* [orderedlist/minimal](https://github.com/orderedlist/minimal)

* [al-folio](https://github.com/alshedivat/al-folio)
