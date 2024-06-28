---
layout: blog-post

title:  "Jekyll Build Installation Website Code "
date:   2023-11-18 17:35:09 +0600
categories: [Jekyll, Code, Website]
keywords: Jekyll  Code Website
description:  Jekyll Website code to strat a jekyll project
image: "https://tds-images.thedailystar.net/sites/default/files/styles/big_202/public/images/2023/07/13/facebook_thumbnail_8.png"

team:
  name: Ahmed Sharif Khan Noor
  tag: Chief Editor / Blogger
  subtitle: Digital Marketer and Social Media Manager
  username: ahmed_sharif_khan
  permalink: ahmed-sharif-khan
  date: 2023-10-12 17:35:09 +0600
  message: |
        There live the blind texts. Separated they live in Bookmarksgrove right at the coast of the Semantics, a large language ocean.
  image: https://lh3.googleusercontent.com/pw/ADCreHd8bz4D53_B3dnZqgyI6lKQ8guUguy3xrJpukvzeMa3s2Ea1-4FSCoAB4TGGJ2PVh2VWacgpBdyAP6Lm4xdU1Stdff6PvXlO5Uuko9dsEGh5mkNBPhAJmeAhpWyOJlzRjv5Ahag3bBo7RBfa4o1UfD6=w480-h480-s-no-gm?authuser=0
  categories: [Graphic Design, Photoshop, Adobe Photoshop, Social Media Banner Design]

social_media:
  - name: facebook
    username: https://www.facebook.com/ahmedsharifkhannoor
  - name: twitter
    username: https://www.twitter.com/maxnoor87
  - name: instagram
    username: https://www.instagram.com/ahmedsharifkhannoor
  - name: linkedin
    username: https://www.linkedin.com/in/ahmedsharifkhannoor
  - name: behance
    username: https://www.behance.net/ahmedsharifkhannoor
  - name: dribble
    username: https://dribble.com/ahmedsharifkhannoor
  - name: pinterest
    username: https://ar.pinterest.com/ahmedsharifkhannoor
  - name: web
---

## To Start A New Project

```
jekyll new .
```

Conflict: E:/NextJs/CodeNinja exists and is not empty. Ensure E:/NextJs/CodeNinja is empty or else try again with `--force` to proceed and overwrite any files.

```
jekyll new . --force
```

```
bundle exec jekyll serve
```

```
 bundle exec jekyll serve --livereload
```

Pass the --livereload option to serve to automatically refresh the page with each change you make to the source files: bundle exec jekyll serve --livereload

```
bundle update github-pages
```

 **Could not find gem 'github-pages'.**

```
bundle install
```

if this is not working then

```
bundle update
```

ruby 3 is not come with webrick

```
bundle add webrick
```

in the gemfile

```
gem "github-pages", group: :jekyll_plugins
```

**_config.yml file configatation**

```
logo: AHMED'S WORLD
title: Ahmed world is a portfolio site
email: youremail@mail.com
start_year: 2023
current_year: { { site.time | date: "%Y" } }
description:
```

**URL configaraton**

```
baseurl: /blog  # the subpath of your site, e.g. /blog
url: http://example.com  # the base hostname & protocol for your site, e.g. http://example.com
```
  
**Social follow button**

```
facebook_username: https://www.facebook.com/ahmedsharifkhannoor
twitter_username: https://www.twitter.com/maxnoor87
instagram_username: https://www.instagram.com/ahmedsharifkhannoor
linkedin_username: https://www.linkedin.com/in/ahmedsharifkhannoor
github_username: https://www.github.com/ahmedsharifkhan
youtube_username: https://www.youtube.com/channel/UCBfIS1RdIpSoS1e75LXJuxw
```
  
```
defaults:
- scope:
path: ""
type: "posts"
values:
permalink: "/blog/:title/"
```
  
```
collections:
portfolio:
output: true
permalink: /portfolio/:path/
```
**Page URL Layout**

```
header_pages:
- title: Home
url: /
- title: Blog
url: /blog
- title: About
url: /about
- title: Contact
url: /contact
- title: Portfolio
url: /portfolio
```
  
```
google_analytics_id: G-W5KN8DPXQ9
facebook_pixel_id: 1234567890
```
  
```
gems:
- jekyll-sitemap
```

```
theme: minima
plugins:
- jekyll-admin
- jekyll-sitemap
- jekyll-feed
```
  
```
pagination:
enabled: true
per_page: 4
permalink: '/:num/'
```

**To watch on mobile use this code**

 ```
host: 0.0.0.0
port: 4000
```

**Code copy and hightlight code**
css code:
<!-- code show -->
```
<style>
    pre {
        background-color: #272A3D;
        background-image: initial;
        background-position-x: initial;
        background-position-y: initial;
        background-size: initial;
        background-repeat-x: initial;
        background-repeat-y: initial;
        background-attachment: initial;
        background-origin: initial;
        background-clip: initial;
        border-radius: 15px;
        box-shadow: 0 4px 30px rgba(0, 0, 0, 0.5);
    }
    pre code {
        display: block;
        padding: 1em;
        overflow-x: auto;
        /* background: linear-gradient(to right, #614294, #8C4E9E); */
        /* Set the background color to black */
        color: #fff;
        /* Set the text color to white */
    }
    ::selection {
        background-color: #464da4;
        /* Green color */
    }
    .copy-code-button {
        background-color: #A4C639;
        color: #0f0f0f;
        border-radius: 15px;
        margin-top: 1px;
        padding: 5px 10px;
        cursor: pointer;
        transition: background-color 0.3s ease, transform 0.3s ease;
    }
    .copy-code-button:hover {
        background-color: #7FA11D;
        transform: scale(1.1);

    }
</style>
```

**JavaScript code**

```
<script>
  document.addEventListener('DOMContentLoaded', (event) => {
    const codeBlocks = document.querySelectorAll('pre code');

    codeBlocks.forEach((codeBlock) => {
      const container = document.createElement('div');
      container.className = 'copy-code-container';

      const button = document.createElement('button');
      button.className = 'copy-code-button primary_btn'; // Add the 'primary_btn' class here
      button.textContent = 'Copy Code';

      button.addEventListener('click', () => {
        const textArea = document.createElement('textarea');
        textArea.value = codeBlock.innerText;
        document.body.appendChild(textArea);
        textArea.select();
        document.execCommand('copy');
        document.body.removeChild(textArea);

        // Change the button text to "Copied!" for a short duration
        const originalText = button.textContent;
        button.textContent = 'Copied!';
        setTimeout(() => {
          button.textContent = originalText;
        }, 1000); // Adjust the duration as needed
      });

      container.appendChild(button);
      codeBlock.parentNode.insertBefore(container, codeBlock.nextSibling);
    });
  });
</script>
```

**Simple copy code**

```
<script>
document.addEventListener('DOMContentLoaded', (event) => {
    const codeBlocks = document.querySelectorAll('pre code');

    codeBlocks.forEach((codeBlock) => {
        const button = document.createElement('button');
        button.className = 'copy-code-button';
        button.textContent = 'Copy Code';

        button.addEventListener('click', () => {
            const textArea = document.createElement('textarea');
            textArea.value = codeBlock.innerText;
            document.body.appendChild(textArea);
            textArea.select();
            document.execCommand('copy');
            document.body.removeChild(textArea);
        });

        codeBlock.parentNode.insertBefore(button, codeBlock.nextSibling);
    });
});
</script>
```
