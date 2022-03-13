# PicoCMS-slider-theme

A picoCMS theme, all your pages are embedded in a slider.

## Feature

A simple [picoCMS](https://github.com/picocms/Pico) theme :
+ All your page embed in a slider
+ Table of Content
+ Tagline in header.

## Install, Pico, version 2.x

Copy the content of the `slider` directory in the `themes` folder of your **Pico** installation and change the following setting within your `config.yml`:

```yaml
theme: slider
```

## Settings

### Index
In the `index.md` of the slider theme. The content and one image below.

```
---
style: slide
title: Welcome to the Slider Theme for picoCMS
image: img.jpg
---
```
### Other pages

The other pages are divided in 3 vertical zones. You can put your content in one of the 3 zone using the `content_vposition` in the yaml metadata :
    + 1 is for above -- content is center
    + 2 is for the middle
    + 3 is for below -- content is center
    
You can add images to your slides using yaml metada :

```
image: 
 - img4.jpg
 - img5.jpg
```

They will appear in the middle zone. If the content is also in the middle zone (`content_vposition: 2`), you can choose the position of the content in relation to the images with the `content_hposition`.


## Additional Settings 

More settings are available using the `_meta.md` file in your `content` folder.

```
---
Logo: %theme_url%/img/pico-white.svg
Tagline: Making the web easy.
Social:
    - title: Visit us on GitHub
      url: https://github.com/psic/PicoCMS-slider-theme
      icon: octocat
TOC: 1
---
```

+ `Logo`: setting a logo at the bottom of the page,
+ `Tagline`: setting a tagline below the site title,
+ `Social`: List of social links (title, url and icon (using `fontello.css`)) on the footer of each page,
+ `TOC`: Set it to `1`, if you want a table of content.

## Demo

demo : [slider.web-en-royans.fr](http://slider.web-en-royans.fr/)
