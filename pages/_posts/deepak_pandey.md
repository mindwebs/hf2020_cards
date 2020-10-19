---
title: Deepak Pandey
institution: DSC KGEC
interests: [Fullstack Web Development, Coding, Debugging]
socials: [
    {
        name: 'Facebook',
        url: 'https://www.facebook.com/profile.php?id=100005101688013'
    },
    {
        name: 'Github',
        url: 'https://github.com/deepak821'
    },
]
image: 'https://avatars2.githubusercontent.com/u/55989361?s=460&u=c4876d14fa0871dbaf6ce92066769058b6c9090c&v=4'
layout: blog
---

This is a default card template. All the fields mentioned on the top are required to stay to our app not to fail. Please change the `title` to be **YOUR NAME** and the `institution` to be **YOUR COLLEGE/THE INSTITUTION YOU ARE WORKING WITH**. You can visit [our repo](https://github.com/mindwebs/hacktoberfest_2020_participation_cards) to add your own page and cards.


You can provide an image for your card in the page by simply mentioning the `image` property in the headers. For that place your image at static folder and mention the `/image_name.ext` to make the image appear on your card.

If similarly you want to have an image on your page you can do the same thing, upload to the static folder and link it via markdown:

![Our Logo Again](https://mindwebs.org/img/logo.png)

Syntax for this is: 

```
![Our Logo Again](https://mindwebs.org/img/logo.png)
```

In case you can't get your pictures online, you may use the static folder like this:

![Our Logo Third time](/mw.png)



```
![Our Logo Third time](/mw.png)
```


---


You can also provide some social media links of your choice in the `socials` field in the header.

An header with all the fields will look like:


```
---
title: Mind Webs
institution: Mind Webs
interests: [Fullstack Web Development]
socials: [
    {
        name: 'Facebook',
        url: 'https://www.facebook.com/mindwebs'
    },
    {
        name: 'Github',
        url: 'https://github.com/'
    },
    {
        name: 'Webpage',
        url: 'https://mwv.net.in/'
    }
]
image: '/mw.png'
layout: blog
---
```
