# Frescobaldi website

The website is built using [Mkdocs](https://www.mkdocs.org/) and the
[mkdocs-material theme](https://squidfunk.github.io/mkdocs-material/).
You can install them using pip:

    pip3 install --user mkdocs mkdocs-material

When you edit the website content, you should run the server in order to
see the changes on browser while you write the markdown files:

    mkdocs serve

When your work is done, you can build the static website:

    mkdocs build

Mkdocs has built-in support to deploy the static site to Github Pages:

    mkdocs gh-deploy

The static site of this repository is currently deployed at
<https://fedelibre.github.io/frescobaldi.org-mkdocs/>.


## TODO

This is a work in progress.

### Add content

We should discuss what to use from the existing user guide and how to
restructure the content.

Mkdocs does not support variables (as in our user guide) within Markdown files.
Check [issue 304](https://github.com/mkdocs/mkdocs/issues/304).

### LilyPond code syntax highlight

Urs suggested writing a Mkdocs plugin to preprocess lilypond snippets
with `python-ly` highlighter.

Another option would be writing a lilypond highlighter for Pygments, see
[CodeHilite extension](https://squidfunk.github.io/mkdocs-material/extensions/codehilite/).

### Content translation

Mkdocs does not currently support content translation.
See the discussion in [issue 211](https://github.com/mkdocs/mkdocs/issues/211#issuecomment-466420384).
