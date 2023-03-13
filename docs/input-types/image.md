---
title: Image
---
An **image picker** can be created by using the following strings as a frontmatter key (gray can be any string):

- image
- *featured*_image

Frontmatter fields with the above keys provide a file selector that filters all image files from the uploads directory. Selecting an image will result in front matter like the below:

    image: "/uploads/yourimagename.jpg"
