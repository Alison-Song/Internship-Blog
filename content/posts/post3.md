---
title: "Wednesday Week1"
date: 2020-01-15
description: "Hugo & VScode"
tags: [hugo, VScode]
---



Try to learn something new every day! It's [Hugo][] and [VScode][] today.  

## Hugo  

Hugo is one of the most popular **open-source static site generators**, which has amazing speed and flexibility. By Hugo, I can build static pages and create a new web site, such as my own blog. It really sounds attractive.  

In order to get this, I should install Hugo and learn some commands. So there we go.

1. To verify the new install, use  

        hugo version  
    
    You can see something ike  
    
        Hugo Static Site Generator v0.62.2/extended windows/amd64 BuildDate: unknown  
2. To create a new site, type the command  

        hugo new site test  
    
    Then it will create a new Hugo site in a new folder called `test`.

3. What makes Hugo popular is that you can choose a **theme** you like or you need from the [themes.gohugo.io].  I write this blog using the theme called [Ezhil][], which is really user-friendly.  
After you choose your theme, download it from Github and add it to your site's `theme` directory  

        cd quickstart
        git init
        git submodule add https://github.com/vividvilla/ezhil.git   
    Then, add the theme to the site configuration  

        echo theme = "ezhil" >> config.toml  
    You can also add it manually.
    Now you can use the theme you want.  
4. Now you actually have a site and a beautiful theme, but it is just a vacant shell, you need to add some content in it.  

    You can create a new **markdown file** and wirte your content in it  

        hugo new test.md     

    You can also do it manually.  
    Then, 

## VScode  



**************************





[Hugo]: https://gohugo.io/
[VScode]: https://code.visualstudio.com/
[Ezhil]: https://github.com/vividvilla/ezhil
