# Chongtian Gao's Blogs
I use (Astro Resume Theme)[https://github.com/wasutz/astro-resume-theme] as the base theme to build my personal website. I extended the original theme to support tags.

## Notes
### All mdx or md files must contain the below metadata at the beginning of the file

```
---
title: "Hello World"
description: "Hello World from Astro. "
datetime: "2025-02-25"
image: "/blog_assets/sdet.png"
url: "/blog/hello-world"
tags:
  - astro
  - test
---
```

- title: this is the Title of the blog
- description: this is the sub-title shown in the blog list
- datetime: the date format shall be "yyyy-mm-dd"
- image: this is the cover image of the blog. Save the image in the public/blog_assets folder or other folder under /public. The path to the image should **include the leading slash "/"**
- url: in the format of "/blog/uid_of_the_blog"
- tags: a list of tags

### How to refer an image inside the markdown
Use this syntax:

```
![alt text](path to the image)
```

Save the image in the public/blog_assets folder or other folder under /public. The path to the image must **include the leading slash "/"**, for example, /blog_assets/sdet.png 