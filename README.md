# Frollo's blog

This blog is based on [Chirpy Starter](https://github.com/cotes2020/chirpy-starter), it adds some new functionalities.

## Features

### PDF embed

It's possible to embed a PDF at the end of the page by using the front matter key `embedded_pdf_filename`.

### Books

Books are essentially (ordered) multipage posts, so if you have a long topic to talk about, you can divide it in multiple "chapters", each chapter links to the previous and next chapter and add a table of contents for navigation. The books chapters won't clutter automatically your posts, you can decide to create a post and link it to a book using `book-id` in the preamble. Chapters start from number 1.

In this repo you have an extra directory `_chapters`. The `_chapters` directory contain the chapters of all books, each chapter has these extra front matter keys:

- `book-id`: The id of the book. For example, `MyFantasyBook`.
- `number`: The number of the chapter, the first chapter must be `1`.

You can give any name to the files in `_chapters`, but it's a good practice to start the name with the `book-id`, for example `MyFantasyBook-01-The-Beginning`, if you add also the chapter number after the book id, the files are easier to sort alphabetically.

## Install

You can follow the [official installation method of Chirpy](https://chirpy.cotes.page/posts/getting-started/), or follow mine.

Follow these steps:

- Install ruby and bundler
- Clone this repo
- Enter the repo directory
- (Recommended) Set bundler to work locally: `bundle config set --local path vendor/bundle`
- Run `bundle install`

## Usage

First, check out [Chirpy theme's docs](https://github.com/cotes2020/jekyll-theme-chirpy/wiki).

- For development, run `bundle exec jekyll serve --livereload`
- For production, run `JEKYLL_ENV=production bundle exec jekyll build` or use Github Actions as described in the [Chirpy docs](https://chirpy.cotes.page/posts/getting-started/#deploy-using-github-actions).

## TODOs

Enhancements:

- Make it possible to attach any file to a post
- The current way of storing book chapters is ugly, I would like to have directories named with the `book-id` and inside of them the actual chapters.
