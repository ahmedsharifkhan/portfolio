---
layout: blog-post

keywords: Health  Travel  Life Style
date: '2023-10-25 02:33:00 +0600'
categories:
- Digital Marketing
- Marketing
- SEO
youtubeid: OTxz8hqdtEk
title: How to set up tawk.to for Google Analytics 4 tracking with Google Tag Manager
description: Google Analytics tracking allows you to learn more about your visitors’ behavior on your site and how they communicate with you
image: https://tds-images.thedailystar.net/sites/default/files/styles/big_202/public/images/2023/10/19/dalle_2023-10-19_19.19.51_-_vibrant_landscape_image_of_two_brown-skinned_urban_bangladeshi_girls_in_their_teens_sitting_on_a_city_bench._one_holds_a_smartphone_and_they_both_dan.png

team:
  name: Kayla Bryant
  subtitle: Digital Marketer and Social Media Manager
  username: kayla_bryant
  tag: Chief Editor / Blogger
  permalink: kayla-bryant
  date: 2023-10-12 17:35:09 +0600
  message: |
      There live the blind texts. Separated they live in Bookmarksgrove right at the coast of the Semantics, a large language ocean.
  image: /assets/images/person_4.jpg
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

---

Google Analytics tracking allows you to learn more about your visitors’ behavior on your site and how they communicate with you. You can set up Google Analytics tracking for your widget with Google Tag Manager to track custom events — for example when a chat starts or ends.

Prerequisites

Before you get started, you’ll need to have the following:

  

1.  A Google Analytics Account and Property
2.  A Google Analytics Data Stream
3.  A tag for the  [tawk.to](http://tawk.to/?_gl=1*8xqfv6*_ga*MTQxNzE2MzQ2LjE3MDk0ODk5MzU.*_ga_ZJL9LF36Z8*MTcxMDQ0MjA5MS41LjEuMTcxMDQ0NjA3Ni4wLjAuMA..)  widget in Google Tag Manager. If this has not yet been set up, follow the steps in this article:  [How to add the tawk.to widget with Google Tag Manager](https://help.tawk.to/article/how-to-add-the-tawkto-widget-with-google-tag-manager)  
    

Setting up Google Analytics

How to set up your Google Analytics Configuration

1 - Create a new tag for adding the Google Analytics Configuration Tag. Make sure to rename the tag (e.g. GA - config).

![](https://tawk.link/521727297ca1334016000005/kb/attachments/EXNVk-J6Ho.png){: width="100%" height="auto"}

2 - Click the  **Tag Configuration**  pane and a new panel will appear.

![](https://tawk.link/521727297ca1334016000005/kb/attachments/hE1dK6UaNg.png){: width="100%" height="auto"}

3 - In the configuration panel, select  **Google Analytics GA4 Configuration**.

![](https://tawk.link/521727297ca1334016000005/kb/attachments/siB8Gpv5Y2.png){: width="100%" height="auto"}

4 - In the form, provide the  **Measurement ID**. You can find this in your Google Analytics account.

![](https://tawk.link/521727297ca1334016000005/kb/attachments/4sJVJ9VsNo.png){: width="100%" height="auto"}

5 - Now, click the  **Triggering**  pane to choose a trigger.

![](https://tawk.link/521727297ca1334016000005/kb/attachments/ugxhS5yjiD.png){: width="100%" height="auto"}

6 - In the triggering panel, select  **All Pages**  to allow the tag to trigger on every page on which Google Tag Manager is installed.

![](https://tawk.link/521727297ca1334016000005/kb/attachments/2067CH2hph.png){: width="100%" height="auto"}

7 - Click **Save**  to create the tag.

![](https://tawk.link/521727297ca1334016000005/kb/attachments/DhcRk5UYJ4.png){: width="100%" height="auto"}

Creating Custom Events For Google Analytics

Next, we’ll use GTM to set up a custom event.

  

As an alternative, you can use our JS API and the gtag function loaded with the global site tag for GA. Learn more in this article:  [How to set up tawk.to for Google Analytics tracking](https://help.tawk.to/article/how-to-set-up-tawkto-for-google-analytics-tracking)  

1 - Create another tag and now select  **Google Analytics GA4 Event** as the  **Tag Configuration**.

![](https://tawk.link/521727297ca1334016000005/kb/attachments/i-H7UuW6mz.png){: width="100%" height="auto"}

2 - In the form, for  **Configuration Tag**, select the  **Google Analytics GA4 Configuration**  tag we created earlier. For the  **Event Name**, put in the custom event that you want to track. (ex. chat_started).

![](https://tawk.link/521727297ca1334016000005/kb/attachments/z0bx9c8S4t.png){: width="100%" height="auto"}

3 - We’ll create a custom trigger for the tag. Click the  **+** button to open a new panel for trigger creation.

![](https://tawk.link/521727297ca1334016000005/kb/attachments/jb8dJyswDb.png){: width="100%" height="auto"}

4 - In the panel, change the trigger name to your liking (ex. Custom -  [tawk.to](http://tawk.to/)  chat started) and click  **Save**. Click the  **Trigger Configuration**  pane, and another panel will appear.

![](https://tawk.link/521727297ca1334016000005/kb/attachments/W4hL4n1CS7.png){: width="100%" height="auto"}

5 - In the panel, scroll down and select  **Custom Event** as the trigger type.

![](https://tawk.link/521727297ca1334016000005/kb/attachments/SnzOuNvKLd.png){: width="100%" height="auto"}

6 - In the form, input the event name for the custom event you want to track and click **Save**  to create the trigger.

![](https://tawk.link/521727297ca1334016000005/kb/attachments/-xcoIhzJJJ.png){: width="100%" height="auto"}

7 - Finally, click the  **Save**  button to complete the tag creation.

![](https://tawk.link/521727297ca1334016000005/kb/attachments/Y2M0E9ZuUk.png){: width="100%" height="auto"}

Setting up a tag for using JS API and a Custom Events trigger

In this section, we’ll provide a sample for triggering the  **chat_started**  custom event we created earlier by using the JS API  **onChatStarted**.

  

**Note:** Before creating a new tag, check for any preexisting tags that are using our JS API. If you already have a tag in place, you can add the additional logic there instead of creating another tag.

  

For example, if you want to add the tracking to the onChatStarted function but you already have an existing tag that uses the onChatStarted function, you can simply add it to the current function as in the following example:

```
Tawk_API.onChatStarted = function () {
  // current existing logic here

  // add the tracking after the existing logic here
  dataLayer.push({
    event: 'chat_started'
  });
}
```

1 - Create a new tag and select Custom HTML as the tag type.

![](https://tawk.link/521727297ca1334016000005/kb/attachments/E7aElDT3Br.png){: width="100%" height="auto"}

2 - In the  **HTML**  field, enter the following code block. Do note that the event property’s value should be equal to the  **Event Name**  that you inputted earlier when creating the custom event tag.

```
<!-- Code for tawk.to to trigger custom events from dataLayer and send to Google Analytics -->
<script type="text/javascript">
var Tawk_API=Tawk_API || {};
Tawk_API.onChatStarted = function () {
  dataLayer.push({
    event : 'chat_started' // value here must be equal to the value set on the custom event tag and trigger
  });
}
</script>
```
![](https://tawk.link/521727297ca1334016000005/kb/attachments/oJiCsi96Rs.png){: width="100%" height="auto"}

3 - In Triggering, select  **All Pages**  to allow the tag to trigger on every page on which Google Tag Manager is installed.

![](https://tawk.link/521727297ca1334016000005/kb/attachments/NZyuFcCxs2.png){: width="100%" height="auto"}

4 - Click **Save**  to complete the tag creation.

![](https://tawk.link/521727297ca1334016000005/kb/attachments/74RHdeEoQe.png){: width="100%" height="auto"}

Check to see if the GA Event tag has been triggered

1. In your tag manager dashboard, click  **Preview**. A new window will open allowing you to connect Google Tag Manager to your site.

  

2. Enter your website URL. The URL you enter will open in a new window.

  

3. Go back to the tab/window where you opened the  **Preview**  page. You should be able to see that your  **Google Analytics: GA4 Event** hasn’t been fired yet.

![](https://tawk.link/521727297ca1334016000005/kb/attachments/EWRfzDPXDR.png){: width="100%" height="auto"}

3. To fire the tag, we’ll trigger it using the custom event we created earlier (which, in this example, is triggered when a chat is started).

  

4. Once we’ve triggered our  **OnChatStarted**  JS API, that should send an event to the  **Data Layer**  which now triggers the  **Google Analytics: GA4 Event** tag.

![](https://tawk.link/521727297ca1334016000005/kb/attachments/C9hejmF6o0.png){: width="100%" height="auto"}

Verify the event has been triggered on the GA4 dashboard

1. In your GA4 dashboard, navigate to  **Reports**  ➞  **Realtime Overview**.

  

2. From there, you’ll be able to see under the  **Event count**  by **Event name**  card that Google Analytics was able to receive the  **chat_started** event.

![](https://tawk.link/521727297ca1334016000005/kb/attachments/spB_pgAJPH.png){: width="100%" height="auto"}

Mark the Custom Event as a Conversion

1. In your GA4 dashboard, navigate to  **Configure**  ➞  **Events**. The events that were received by Google Analytics will show up there within 24 to 48 hours.

![](https://tawk.link/521727297ca1334016000005/kb/attachments/sLspvJX2MN.png){: width="100%" height="auto"}

2. To mark the  **chat_started**  event as a conversion, simply enable the switch under the  **Mark as conversion**  column for that record.

![](https://tawk.link/521727297ca1334016000005/kb/attachments/uAVHkQ9JGT.png){: width="100%" height="auto"}

3. After enabling, you should now see the event under  **Configure**  ➞  **Conversions**.

![](https://tawk.link/521727297ca1334016000005/kb/attachments/vAJwMH-lz1.png){: width="100%" height="auto"}