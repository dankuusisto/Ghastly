# Spook
-----

Spook is a markdown blog with a Ghost-like theme for the very lazy blogger. 

## Installation

Clone the repository, run `composer install` and edit `config.php`. 

Create posts in `posts/` in the format of `2014-12-28-my-blog-post-title.md`.

A post should have a jekyll-like front matter. An example post would look like:

    -----
    title: My blog post title!
    tags: something, stuff
    -----

    Lorem ipsum dolor sit amet...

The `tags:` line is optional.

## Themes

Spook uses the `spooky` theme by default. You can copy it to a folder and rename it to something else to make your own theme. You can modify the html files however you like. Spook uses the Twig template engine.

Your template must have a `layout.html` file and a `single_post_layout.html` file.

### Template Variables

Spook exposes the following variables for you to use in your templates:

Variable              | Explanation
----------------------|:------------
 `posts`              | This is an array of posts
 `post`               | A single post
 `post.metadata.date` | The date of a post
 `post.metadata.tags` | The tags of a post
 `post.metadata.title`| The title of a post
 `post.content`       | The html content of a post
 `blog_title`         | The name of your blog
 `blog_author`        | The name of the blog author
 `blog_url`           | The url your blog is located at
 `blog_description`   | The description of your blog if you gave one