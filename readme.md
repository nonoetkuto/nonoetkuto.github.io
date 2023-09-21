# Nono et Kuto - L'actualité e-sport (draft)

## Installation procedure & content management

### Install Hugo using winget
```shell
winget install Hugo.hugo.Extended
hugo --version # Check if hugo is correctly installed
```

Once hugo is installed, checkout the git repository on your machine.

### Run locally
```shell
cd <project_dir>
hugo server
# or
hugo server -D # Run locally with content marked as draft
```

### Create a blog post
```shell
cd <project_dir>
hugo new content posts/<blogpost_dir>/index.md
```

`blogpost_dir` must be named as following: `YYYYMMDD-your-project-title`

For example:
- `20160107-lancement-nk`
- `20170922-test-nentendo-switch`
- `20230921-lideal-cest-de-niro`

`index.md` will be the content of your blog post.

### Add images on your blog post

Images should be stored inside `content/posts<blogpost_dir>/images`. For example

```
content
 \__posts 
 |  \__20230921-article-1
 |  |  |--index.md
 |  |  \__images
 |  |  |  |--img1.jpg
 |  |  |  |--img2.jpg
 |  |
 |  \__20230921-article-2
 |  |  |--index.md
 |  |  \__images
 |  |  |  |--img1.jpg
 |  |  |  |--img2.jpg
```

Therefore inside of the respective `index.md` file, you can link to images as follows:
- `![my-image-1](images/img1.jpg)`
- `![my-image-2](images/img2.jpg)`

### Blog post template

```
+++
title = "My blog post title"
date = 2023-09-21T10:47:47+02:00
excerpt = "My blog post subtitle"
tags = ['le', 'plus', 'impotant', 'c', 'le', 'pizik]
draft = true
+++

# Section 1
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker incl

> Neque porro quisquam est qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit...

Sed ut perspiciatis unde omnis iste natus [error](https://www.youtube.com/watch?v=_XRnENg_QI0) sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo.

![](images/2.png)
*Caption here*

__NK__

```
