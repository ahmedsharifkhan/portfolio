---
layout: blog-post

title:  "What is server-side tagging? Tagging is the act of adding snippets of code on a website for measurement"
date:   2023-10-12 17:35:09 +0600
categories: [Health,  Travel, Life Style]
keywords: [Health  Travel Life Style]
description: The answer is no but it can greatly complement and improve the work done by client-side tags. With server-side tagging, an additional layer of control is inserted between the user and the marketing vendor. This layer allows you to control the exact composition of data that the vendors receive.
image: "https://tds-images.thedailystar.net/sites/default/files/styles/big_202/public/images/2023/10/12/online_posts-9.jpg"

team:
  name: Thomas Crawford
  tag: Chief Editor / Blogger
  subtitle: Digital Marketer and Social Media Manager
  username: thomas_crawford
  permalink: thomas-crawford
  date: 2023-10-12 17:35:09 +0600
  message: |
      There live the blind texts. Separated they live in Bookmarksgrove right at the coast of the Semantics, a large language ocean.
  image: /assets/images/person_6.jpg
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

What is server-side tagging?
Tagging is the act of adding snippets of code on a website for measurement by a marketing team, marketing partner, or a tool like Google Analytics.

Client-side tagging: The tags on your website or app are executed on the user’s device.
Server-side tagging: The tags on your website or app are executed on a server.
Tag Manager for web vs on a server
Before server-side tagging, client-side tagging was your only option to place and execute tags. You might wonder: "Does server-side tagging replace client-side tagging?"

The answer is no but it can greatly complement and improve the work done by client-side tags. With server-side tagging, an additional layer of control is inserted between the user and the marketing vendor. This layer allows you to control the exact composition of data that the vendors receive.

Additional benefits include:

Improved page speed as the amount of third-party code loaded in the user's browser is greatly reduced.
Content security policies can be made more restrictive, as the browser no longer needs to communicate directly with vendor domains.
Privacy is improved because personal data such as the user's IP address can be removed from the data dispatched to the vendor.
Cookies can be made more secure and durable because they are set on your own domain and are not set by the JavaScript on the page.
Differences between a server container and a web container
Server containers Web containers
Server containers run in the server Web containers run in the browser
Server containers digest HTTP requests Web containers use the dataLayer
Server containers only use sandboxed JavaScript Web containers can deploy HTML tags and run custom JavaScript code at runtime
Server containers can incur costs from maintaining the server environment Web containers are cost-free
How server-side tagging works
In the context of this course, the tags need to be placed in a Tag Manager server container.
A server container is a JavaScript application that runs in a server environment on Node.js.
The application is packaged and distributed as a Docker image, which means it is compatible with many different server environments and cloud services.

A Tag Manager server container works together with a Tag Manager web container or the gtag.js library. The client-side libraries have mechanisms to collect data from the web browser and dispatch it to the server-side tagging environment.


![What is server-side tagging?](https://developers.google.com/static/tag-platform/learn/images/how-sst-works.png){: width="100%" height="auto"}



Diagram showing how the GA 4 client and the web container interact
Term Definition
Client Clients are a Tag Manager resource available only in server containers.

The main purpose of a client is to parse an incoming HTTP request and generate an event data object for tags to utilize.

A single incoming HTTP request can be "claimed" by only one client. As soon as a client claims the request, no other client can be activated for that request anymore.
Request A request refers to the HTTP request that is sent to the server container. The only way to make the server container process data is to send HTTP requests to it. Once the server container completes its work, it will dispatch a response back to the HTTP request source.
Event Data The client parses the incoming HTTP request into a standardized Event Data format.

Event data is analogous to the "Data Layer" in the web container. You can use the generated event data objects to fire and enrich your server-side tags.
Triggers Triggers in a server container are always related to the event data object generated by the client. There are no click or scroll triggers, for example.
Tags Tags can be used only if the client generates an event data object. Not all clients do this, so you need to be aware of how clients work when installing them in the server container.

The built-in Google Analytics 4 (GA4) client that we'll use in this walkthrough generates a standardized event data object, which makes it easy to fire tags with the incoming GA4 request.
Variables Variables in a server container typically reference items in the event data object. You can configure variables to pull in values directly from the incoming HTTP request (such as request headers). You can create custom templates for even more flexibility.
Where to place tags?
If the tags you deploy in a server-side tagging environment need to know what the user does on a web page or in an app, then some tags still need to run in the browser or app. Since your server container runs in the server-side environment, it has no access to what happens on a web page or an app. The container on your web page or app communicates to the server container with network requests.

For example, if you want to collect data about user interactions on a web page, such as clicks, scrolls, and form interactions, you still need the GA4 Configuration tag running in the web browser to dispatch this information to the server-side tagging endpoint. Similarly, if you want to collect custom events that relate to website interactions, you need to place a GA4 Event tag in the Tag Manager web container.

Summary
To recap, a server-container augments functionality of a web container. It allows you to meet privacy requirements more easily while improving your site performance. If your tag relies on activity that happens in the user's browser, place it in the web container. All other tags can be run in a server container.
