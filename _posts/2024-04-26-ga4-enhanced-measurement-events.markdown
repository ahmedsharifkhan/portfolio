---
layout: blog-post

keywords: Health  Travel  Life Style
date: '2024-04-26 02:33:00 +0600'
categories:
- Digital Marketing
- Marketing
- SEO
youtubeid: QmEOPuJr05w
title: GA4 Enhanced measurement events
description: Discover how to enable and disable enhanced measurement events and learn more about which parameters are collected for each event
image: https://tds-images.thedailystar.net/sites/default/files/styles/very_big_1/public/images/2024/04/22/should_social_media_be_our_new_public_square.png

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

Enhanced measurement lets you measure interactions with your content by enabling options (events) in the Google Analytics interface. No code changes are required. When you enable these options for a web data stream, your Google Analytics tag starts sending events right away.

Before turning on the enhanced measurement feature, be sure you understand each option and what enhanced data will be collected. You can also turn off specific measurement options in settings.

You're required to ensure that no  [personally identifiable information](https://support.google.com/analytics/answer/7686480)  is collected.

## Enable or disable enhanced measurement events

1.  In  [Admin](https://support.google.com/analytics/answer/6132368), under  _Data collection and modification_, click  **Data streams**.
2.  Click the name of your data stream.
3.  Under  _Enhanced measurement_, slide the switch  **On**  to enable all options.  
    Click  ![Settings](https://lh3.googleusercontent.com/PzFeiQQaPASuntRuvWiXoqZjQqUj0s0q0w_jI4Nx9vL6x7rGmmS9f-xQr1Kj9S91WMlm=h36)  to edit individual options as needed.

![Enable enhanced measurement slider](https://storage.googleapis.com/support-kms-prod/jSN8lyeZNXQYjaxLguisELX1ojlvMmO3iDEJ){: width="100%" height="auto"}

If you use  [the Google tag](https://support.google.com/analytics/answer/11994839) on your website, you also need to make sure that each event is enabled for automatic event detection for your Google tag. By default, all event types are enabled. [Learn more about your Google tag settings](https://support.google.com/analytics/answer/12131703#Event&zippy=%2Cmanage-automatic-event-detection)

## Events measurement and parameters

The following table explains when events are triggered, and which parameters are collected for each event. You can find enhanced data about each triggered event in the Events report within  [the Engagement topic](https://support.google.com/analytics/answer/10999789). Click the event name in the report for more information on the event.

To understand each event parameter listed below and how each parameter updates a dimension or metric in Google Analytics, see  [Google Analytics event parameters](https://support.google.com/analytics/table/13594742).

Measurement option / event

Triggered...

Parameters

Page views

page_view

each time the page loads or the browser history state is changed by the active site  
  
This event is collected automatically. You cannot turn off collection.  
  
An advanced setting on this option controls whether the event is sent based on browser-history events. This measurement option listens for pushState, popState, and replaceState.

The event populates the [_Views_](https://wordtohtml.net/analytics/answer/9143382#page-screen-metrics) metric. The parameters populate the following dimensions:

-   [_Page location_](https://wordtohtml.net/analytics/answer/9143382#page-screen) (from page_location)
-   [_Page referrer_](https://wordtohtml.net/analytics/answer/9143382#page-screen) (from page_referrer)

page_location (page URL), page_referrer (previous page URL)

Scrolls

scroll

the first time a user reaches the bottom of each page (i.e., when a 90% vertical depth becomes visible)

The event populates the [_Percent scrolled_](https://wordtohtml.net/analytics/answer/9143382#general) dimension.

No parameters are collected

Outbound clicks

click

each time a user clicks a link that leads away from the current domain

By default, outbound click events will occur for all links leading away from the current domain. Links to domains configured for [cross-domain measurement](https://wordtohtml.net/analytics/answer/10071811) will not trigger outbound click events.

The parameters populate the following dimensions:

-   [_Link classes_](https://wordtohtml.net/analytics/answer/9143382#link) (from link_classes)
-   [_Link domain_](https://wordtohtml.net/analytics/answer/9143382#link) (from link_domain)
-   [_Link ID_](https://wordtohtml.net/analytics/answer/9143382#link) (from link_id)
-   [_Link URL_](https://wordtohtml.net/analytics/answer/9143382#link) (from link_url)
-   [_Outbound_](https://wordtohtml.net/analytics/answer/9143382#link) (from outbound)

link_classes, link_domain, link_id, link_url, outbound (boolean)

Site search

view_search_results

each time a user is presented with a search results page, as indicated by the presence of a URL query parameter  
  
By default, the event is triggered based on the presence of one of the following 5 query parameters in the URL:

-   q
-   s
-   search
-   query
-   keyword

You can optionally configure this event to look for other URL query parameters.

The search_term parameter populates the [_Search term_](https://wordtohtml.net/analytics/answer/9143382#general) dimension.

search_term, optionally ‘q_<additional key="">’ (where <additional key=""> matches an additional query parameter you specify to be collected under advanced settings).

Note: This event only sends the unique_search_term parameter when it has a value of 1 (i.e. when the string is unique to that session).

Video engagement

video_start

video_progress

video_complete

For YouTube embedded videos that have [JS API support](https://developers.google.com/youtube/player_parameters#enablejsapi) enabled, the following events are triggered:

-   video_start: when the video starts playing
-   video_progress: when the video progresses past 10%, 25%, 50%, and 75% duration time
-   video_complete: when the video ends

The parameters populate the following dimensions:

-   [_Video provider_](https://wordtohtml.net/analytics/answer/9143382#video) (from video_provider)
-   [_Video title_](https://wordtohtml.net/analytics/answer/9143382#video) (from video_title)
-   [_Video URL_](https://wordtohtml.net/analytics/answer/9143382#video) (from video_url)
-   [_Visible_](https://wordtohtml.net/analytics/answer/9143382#general) (from visible)

video_current_time, video_duration, video_percent, video_provider, video_title, video_url, visible (boolean)

File downloads

file_download

when a user clicks a link leading to a file (with a common file extension) of the following types:

-   document
-   text
-   executable
-   presentation
-   compressed file
-   video
-   audio

File extensions that match the following regex will trigger the event:

pdf|xlsx?|docx?|txt|rtf|
|csv|exe|key|pp(s|t|tx)|  
7z|pkg|rar|gz|zip|avi|mov|
|mp4|mpe?g|wmv|
|midi?|mp3|wav|wma

The parameters populate the following dimensions:

-   [_File extension_](https://wordtohtml.net/analytics/answer/9143382#general) (from file_extension)
-   [_File name_](https://wordtohtml.net/analytics/answer/9143382#general) (from file_name)
-   [_Link classes_](https://wordtohtml.net/analytics/answer/9143382#link) (from link_classes)
-   [_Link ID_](https://wordtohtml.net/analytics/answer/9143382#link) (from link_id)
-   [_Link text_](https://wordtohtml.net/analytics/answer/9143382#link) (from link_text)
-   [_Link URL_](https://wordtohtml.net/analytics/answer/9143382#link) (from link_url)

file_extension, file_name, link_classes, link_id, link_text, link_url

Form interactions

form_start

form_submit

'form_start': the first time a user interacts with a form in a session

'form_submit': when the user submits a form

You can use these two events to see how many users started to fill out a form and compare the information to users who submitted the form.

Note: You can only use the parameters in your reports if you [create custom dimensions](https://wordtohtml.net/analytics/answer/10075209) for them.

form_start

-   form_id: HTML id attribute of the <form> DOM element
-   form_name: HTML name attribute of the <form> DOM element
-   form_destination: URL to which the form is being submitted

form_submit

-   form_id: HTML id attribute of the <form> DOM element
-   form_name: HTML name attribute of the <form> DOM element
-   form_destination: URL to which the form is being submitted
-   form_submit_text: text of the submit button, if present
