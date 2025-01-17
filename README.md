# Frollo's blog

This blog is based on [Chirpy Starter](https://github.com/cotes2020/chirpy-starter), it adds some functionalities like books and publications support.

Books are essentially (ordered) multipage posts, so if you have a long topic to talk about, you can divide it in multiple "chapters", each chapter links to the previous and next chapter and add a table of contents for navigation. The books chapters won't clutter automatically your posts, you can decide to create a post and link it to a book using `book-id` in the preable. Chapters start from number 1 (Should I allow for a default value?). 

Publications are posts that embed a PDF file, they are grouped in a separate tab called "publications" (you can easily change the name by renaming the file `notes.md` in the `_tabs` folder), they appear in the timeline (TODO), but not in the home. 

## Install

You can follow the official installation method of Chirpy, or follow mine.

Follow these steps:
- Install ruby and bundler
- Clone this repo
- Enter the repo directory and run `bundle install`
- For development, run `bundle exec jekyll serve --livereload`

## Usage

First, check out [Chirpy theme's docs](https://github.com/cotes2020/jekyll-theme-chirpy/wiki).

In this repo you have the following extra folders: `_chapters`, `_publications`. The `_publications` folder simply contains all the publications (just like the `_posts` folder contains all the posts), while the `_chapters` folder contain the chapters of all book, with the `book-id` in front of the name, I would like instead to have folders named with the book id, because I would get a cleaner folder structure.


