---
layout: blog-post

title:  "Integrating Google Ads with tawk.to"
date:   2023-11-20 5:35:09 +0600
categories: [tawk, Code, Website]
keywords:   tawk Chat Bot
description:  Google conversion tracking gives you valuable insights into how ad clicks lead to valuable customer interactions in tawk.to.
image: "https://tds-images.thedailystar.net/sites/default/files/styles/big_202/public/images/2023/11/20/dalle_2023-11-20_22.53.01_-_a_landscape-oriented_close-up_dramatic_image_showing_the_backs_of_a_diverse_group_of_employees_in_silhouette_protesting_outside_an_office_building.png"

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
    username: https://ahmedsharifkhannoor.blogspot.com
  - name: globe
    username: https://designtgg.blogspot.com/
  - name: person
    username: https://bio.site/ahmedsharifkhannoor
  - name: whatshot
    username: https://www.threads.net/@ahmedsharifkhannoor
  - name: github
    username: https://www.github.com/ahmedsharifkhan
  - name: threads
    username: https://www.threads.net/@ahmedsharifkhannoor
  - name: youtube-play
    username: https://www.youtube.com/channel/UCBfIS1RdIpSoS1e75LXJuxw
---

Google conversion tracking gives you valuable insights into how ad clicks lead to valuable customer interactions in tawk.to.  

  

By creating a conversion action in Google Ads, you can track visitor engagement with the widget.

  

First, you’ll need to set up the conversion action in your Google Ads account and get a piece of code called a tag.

  

Then, to finish setting up conversion tracking, you’ll take a component of the tag and integrate it with the  [tawk.to](http://tawk.to/)  JavaScript API.

  

Finally, you’ll add the new tag to your website.

  

Here's what you'll need before you can set up website conversion tracking:

-   A Google Ads account
-   A website — this is where you'll put the conversion tracking tag
-   Ability to edit the website — either you or your webmaster will need to be able to add the tag to the site
-   A free  [tawk.to](http://tawk.to/)  account

  

**Step 1** - Get the conversion tracking code (tag) from Google Ads

  

Set up a conversion action in your Google Ads account. Then follow these instructions from Google to get your conversion tag:  [Set up conversion tracking for your website - Google Ads Help.](https://support.google.com/google-ads/answer/6095821?co=ADWORDS.IsAWNCustomer%3Dfalse&oco=0)

  

**Step 2** - Install Global site tag

  

If the Google tag isn't installed on all your HTML pages, Copy the tag from your Google Ads account and paste it between the head tags of every page of your website. You only need to install the Google tag once per account, even if you're tracking multiple actions.

```
<!-- Google tag (gtag.js) -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());

  gtag('config', 'G-XXXXXXXXXX');
</script>
```
Step 3 - Get your Google Ads code  
  

Copy the code between script tags from your Google Conversion event code

![](https://tawk.link/521727297ca1334016000005/kb/attachments/plHbs54dqx.png)

**Step 4**  - Place the code  **after**  your  [tawk.to](http://tawk.to/)  widget embed code.

  

Copy the newly created code to the footer of your website, just  **below**  the existing  [tawk.to](http://tawk.to/)  chat embed code. Then  **Save** or  **Publish**  your changes to update the site.
```
<!-- Google Code for tawk.to Chat Conversion -->
<script type="text/javascript">
var Tawk_API = Tawk_API || {};
Tawk_API.onChatStarted = function(){   
       gtag('event', 'conversion', {'send_to': 'AW-xxxxxxxxxx/####################'});
};
</script>
```