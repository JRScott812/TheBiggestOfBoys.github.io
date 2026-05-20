# JRScott812.GitHub.io

This repository contains a simple static site. I converted the site to a Jekyll-compatible structure and added placeholders for future projects.

Local development
-----------------

Requirements: Ruby (2.7+ or compatible), Bundler.

Install dependencies and serve locally:

```bash
gem install bundler
bundle install
bundle exec jekyll serve --livereload
```

Then open http://127.0.0.1:4000 in your browser.

Adding projects
---------------

Create a markdown file in `_projects/` with front matter (title, date, tags, excerpt, image, published).
Set `published: true` to have it appear on the site.