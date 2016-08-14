# Blog

This is my car blog.  It is primarily used as a way for me to take notes and post pictures of the restore process.  It's also nice to be able to share the pictures with people.  

## Setup notes for Ubuntu 16.04

To get [Jekyll](http://jekyllrb.com/) running locally:

* Followed the [Github Pages guide](https://help.github.com/articles/setting-up-your-github-pages-site-locally-with-jekyll/).
* Install ruby-execjs: `sudo apt install ruby-execjs`
* To run the server:
`bundle exec jekyll serve`
* To compress images install [ImageMagick](http://www.imagemagick.org):
`sudo apt install imagemagick`
`convert example.jpg -resize 1024 example.jpg`
`mogrify -resize 1024 *.jpg` to batch resize in place

To run a local Jekyll server without changing the main `_config.yml` file you can create a dev version and specify that config file when you run the server.  The dev version can be added to the `.gitignore` file.

`bundle exec jekyll serve --config _config-dev.yml`
