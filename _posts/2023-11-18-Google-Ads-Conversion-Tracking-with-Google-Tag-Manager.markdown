---
layout: blog-post
author: Ahmed Sharif Khan

team:
  name: Adam Aderson
  tag: Chief Editor / Blogger
  subtitle: Digital Marketer and Social Media Manager
  username: adam_aderson
  permalink: adam-aderson
  date: 2023-10-12 17:35:09 +0600
  author_email: jane.doe@email.com
  message: |
        There live the blind texts. Separated they live in Bookmarksgrove right    at the coast of the Semantics, a large language ocean.
  image: /assets/images/person_2.jpg
  categories: [Graphic Design, Adobe Photoshop, Banner Design]
 
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
# author_name: Jane Doe
# username: ahmed
# author_bio: Web Developer and Blogger
# author_email: jane.doe@email.com
# author_avatar: /assets/authors/author.png
# author_avatar: /assets/authors/profileofnoor.png
# author_avatar: /assets/images/profileofnoor.png


title:  "Google Ads Conversion Tracking with Google Tag Manager"
date:   2023-11-21 5:35:09 +0600
categories: [Tawk, Tracking, Website]
keywords: Tawk Tracking Website Google Tag Manager
description:  Tracking Google Ads conversions with Google Tag Manager
image: "https://tds-images.thedailystar.net/sites/default/files/styles/big_202/public/images/2023/11/20/dalle_2023-11-20_14.03.42_-_an_urban_scene_in_dhaka_north_city_corporation_dncc_depicting_trees_being_numbered_and_mapped_using_the_gprs_system._the_image_shows_workers_in_safe.png"
---

Tracking Google Ads conversions with Google Tag Manager gives you insights into the actions visitors take after viewing an ad on your site.

  

When visitors click your Google Ad, a temporary cookie is stored on their devices. Then, when they complete an action you’re tracking, a new conversion is counted.

  

Follow the steps below to set up Google Ads Conversion tracking in your  [tawk.to](http://tawk.to/)  widget and learn which ads, ad groups, and keywords are bringing the conversions and conversations to your business.

  

1.  Set up a conversion
2.  Set up a Google Adwords Conversion Tracking in GTM
3.  Set up a tag for using the JS API and the Custom Event trigger
4.  Check to see if the Google Ads Conversion Tracking tag has been triggered

Prerequisites

You will need to set up a tag for the  [tawk.to](http://tawk.to/)  widget in Google Tag Manager. If you have not yet done this, follow the steps in this article:  [How to add the tawk.to widget with Google Tag Manager](https://help.tawk.to/article/how-to-add-the-tawkto-widget-with-google-tag-manager)  

Set up a Conversion

1. Log in to your Google Ads account and head over to  **Tools and settings**  ➞  **Measurement**  ➞  **Conversions**. Then, click the  **+** button to add a new conversion.

![](https://tawk.link/521727297ca1334016000005/kb/attachments/lDs2T2bj87.png){: width="100%" height="auto"}

![](https://tawk.link/521727297ca1334016000005/kb/attachments/lDs2T2bj87.png){: width="100%" height="auto"}

2. Select Website as the type of conversion you would like to track.

![](https://tawk.link/521727297ca1334016000005/kb/attachments/9wXrodqE1D.png){: width="100%" height="auto"}

3. Next, it’s time to configure your conversion. Select a category, name your conversion, and input a value representing the impact of the conversion on your business. Then, click  **Create and Continue**.

![](https://tawk.link/521727297ca1334016000005/kb/attachments/MlV7ZfMDw0.png){: width="100%" height="auto"}

4. After creating the conversion, you’ll be presented with options for setting up the conversion tag.

  

Select U**se Google Tag Manager**  and take note of the  **Conversion ID**  and  **Conversion Label**. We’ll be using these later on.

  

Click  **Next**  to finish the creation process.

![](https://tawk.link/521727297ca1334016000005/kb/attachments/T4_hR6ka8X.png){: width="100%" height="auto"}

Set up Google Adwords Conversion Tracking in GTM

1. Create a new tag for adding  **Google Ads Conversion Tracking**. Make sure to rename the tag. Enter your Google Ads  **Conversion ID**  and  **Conversion Label** into their respective fields. Then, click  **Triggering** to select a trigger.

![](https://tawk.link/521727297ca1334016000005/kb/attachments/4ongVHhdyK.png){: width="100%" height="auto"}

2. Click the  **+**  sign located in the upper-right corner of the panel to create a new trigger.

![](https://tawk.link/521727297ca1334016000005/kb/attachments/09s9pvJ5Da.png){: width="100%" height="auto"}

3. Click the  **Trigger Configuration** pane and select  **Custom Event**  as the trigger type. Rename the custom event. Then, in the form, add an E**vent Name** for the conversion tracking and click  **Save** to create the trigger.

![](https://tawk.link/521727297ca1334016000005/kb/attachments/vek3GxG1AZ.png){: width="100%" height="auto"}

4. Next, click the  **create**  link beside the  **Conversion Linker tag missing in container** notification. This will open a panel to create the  **Conversion Linker**  tag. Rename the tag and click  **Save**.

![](https://tawk.link/521727297ca1334016000005/kb/attachments/y2uXOL_tP1.png){: width="100%" height="auto"}

5. Lastly, you’ll be redirected back to the **Google Ads Conversion Linker** tag configuration panel. Click  **Save**  to finalize the creation of the tag.

![](https://tawk.link/521727297ca1334016000005/kb/attachments/Y3e1j4QEsA.png){: width="100%" height="auto"}

Set up a tag for using the JS API and the Custom Event trigger

In this section, we’ll walk through a sample setup triggering the  **chat_started**  custom event we created earlier using the JS API  **onChatStarted**  function.

  

1. Create a new tag and select  **Custom HTML**  as the tag type.

![](https://tawk.link/521727297ca1334016000005/kb/attachments/I-PhjTkF9W.png){: width="100%" height="auto"}

2. In the  **HTM**L field, enter the following code block. The event property’s value should be equal to the  **Event Name**  you entered when creating the custom event tag.

~~~
<!-- Code for tawk.to to trigger the custom events and the Adwords Conversion Tracker tag -->
<script type="text/javascript">
  var Tawk_API=Tawk_API || {};

  // Add all tawk.to JS API related code here. 
  Tawk_API.onChatStarted = function () {
    dataLayer.push({
      event : 'chat_started' // value here must be equal to the value set on the custom event's event name
    });
  }
</script>
~~~
![](https://tawk.link/521727297ca1334016000005/kb/attachments/cw28EShY_k.png){: width="100%" height="auto"}

3. In  **Triggering**, select  **All Pages**  to allow the tag to fire on every page on which Google Tag Manager is installed.

![](https://tawk.link/521727297ca1334016000005/kb/attachments/w0WNKFUYMP.png){: width="100%" height="auto"}

4. Click **Save**  to complete the tag creation.

![](https://tawk.link/521727297ca1334016000005/kb/attachments/VB_FZwu4TD.png){: width="100%" height="auto"}

Check to see if the Google Ads Conversion Tracking tag has been triggered

1. In your tag manager dashboard, click  **Preview**. A new window will open allowing you to connect Google Tag Manager to your site.

  

2. Enter your website URL. The URL you enter will open in a new window.

  

3. Go back to the tab/window where you opened the  **Preview**  page. You should be able to see your  **Google Ads Conversion Tracking**  tag hasn’t been fired yet.

![](https://tawk.link/521727297ca1334016000005/kb/attachments/mHzhTROoDH.png){: width="100%" height="auto"}

4. To fire the tag, we’ll trigger it using the custom event we created earlier (which, in this example, is triggered when a chat is started).

  

Once we’ve triggered our  **OnChatStarted**  JS API, that should send an event to the  **Data Layer** which now triggers the  **Google Ads Conversion Tracking**  tag.

![](https://tawk.link/521727297ca1334016000005/kb/attachments/m3pU8_-g4v.png){: width="100%" height="auto"}
