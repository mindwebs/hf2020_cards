---
title: Abhishek yard
institution: HBTU
interests: [Front End Development, Competitive Coding, Painting, Music]
socials: [
    {
        name: 'Facebook',
        url: 'https://www.facebook.com/people/Abhishek_Yadav'
    },
    {
        name: 'Github',
        url: 'https://github.com/abhi14nexus'
    },
    {
        name: 'Personal Website',
        url: 'https://google.com'
    }
]
image: 'https://images.unsplash.com/photo-1518765829116-c30081bc0cdd?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1050&q=80'
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
