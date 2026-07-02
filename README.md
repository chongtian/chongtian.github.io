# Chongtian Gao's Blogs
I use [Astro Zen Theme](https://github.com/Secd0g/zen) as the base theme to build my personal website. 

## Notes
### All mdx or md files must contain the below metadata at the beginning of the file

```
---
title: "Hello World"
description: "Hello World from Astro. "
pubDate: 2025-02-25
tags: ["astro", "test"]
---
```

- title: this is the Title of the blog
- description: this is the sub-title shown in the blog list
- pubDate: the date format shall be "yyyy-mm-dd"
- tags: a list of tags

### How to refer an image inside the markdown
Use this syntax:

```
![alt text](path to the image)
```

Save the image in the public/blog_assets folder or other folder under /public. The path to the image must **include the leading slash "/"**, for example, /blog_assets/sdet.png 