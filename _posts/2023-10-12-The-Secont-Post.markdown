---
layout: blog-post

title:  "Go ahead and edit it and re-build the site to see your changes"
date:   2023-10-12 17:35:09 +0600
categories: [Travel, Life Style]
keywords: Health  Travel Life Style
description:  After that, include the necessary front matter. Take a look at the source for this post to get an idea about how it works.
image: "https://tds-images.thedailystar.net/sites/default/files/styles/very_big_201/public/images/2023/10/05/smart_nid_data_of_citizens_leaked_in_bangladesh.png"

team:
  name: Nora Layman
  tag: Chief Editor / Blogger
  subtitle: Digital Marketer and Social Media Manager
  username: nora_layman
  permalink: nora-layman
  date: 2023-10-12 17:35:09 +0600
  message: |
      There live the blind texts. Separated they live in Bookmarksgrove right at the coast of the Semantics, a large language ocean.
  image: /assets/images/person_5.jpg
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

#### Client-side and server-side tagging

This page is for marketers and developers who want to decide whether to introduce server-side tagging to complement their current tagging setup.

Google Tag Manager supports two distinct configurations: client-side tagging and server-side tagging.

![Diagram comparing the architecture of client-side tagging and server-side tagging.](https://lh5.googleusercontent.com/BzLp2K4MsrVbeqONBqcvXi0nt7bP3XcpwBQ4bGO7LVX4NbUIYHdgbX0n4nJQk4T8HiU_tJlFQz2LFJ17EOXgsuoI8c4LbWMhOmEslLoy73_vdrprNgjvXSjD691-0KcocHyeYfSvZYZOGbTygr76ugM){: width="100%" height="auto"}

Client-side tagging

Server-side tagging

In client-side tagging, a single container resides on the website or app.

The container holds all tags, triggers, variables, and related code used to measure user interactions.

When a user visits a page, the container is activated and loads the related tags. When the user performs an action that triggers a tag, the event data gets dispatched into one or more HTTP requests from the browser or device to your Google products or advertising partners.

Server-side tagging uses two containers:

-   Web container that resides on the website or app
    
-   Server container that resides in a cloud environment
    

The web container hosts only the tags necessary to monitor and dispatch information about user interactions and generate events as HTTP requests.

The server container accepts all HTTP requests from the web container. In the server container, you can set up processing rules before sending data to your Google products or third-party endpoints.

##enter code here Why should you use server-side tagging?

The purpose of the server container is to provide an intermediary endpoint that you own between the browser or device where events are recorded and the third-party endpoints. The server container complements the web container by handling resource-intensive processing that would normally run in the browser in the client-side tagging configuration. The server container also provides you with the opportunity and the tools to screen, validate and modify data as needed, before sending it on to the analytics and advertising endpoints.

The key benefits of using server-side tag`enter code here`ging are:

-   Reduces the client processing load, improving website and app performance
    
-   Enables you to screen and modify incoming requests to ensure data privacy
    
-   Enables you to validate and normalize data, improving data quality
    

### Improve website or app performance

Server-side tagging improves client performance by reducing the amount of code executed in the browser or app. In client-side tagging, the browser must map each event to one or more HTTP requests, depending on how many endpoints you send the event information to. Therefore, your client might send multiple very similar HTTP requests, which can place a significant load on client resources.

In a server-side tagging setup, the client only has to generate one HTTP request per event that gets sent to the server container. Then, the server container generates and dispatches vendor-specific requests. The result is improved website performance as the client executes less code and dispatches fewer HTTP requests.

To further improve page speed, you can load marketing-related libraries and resources through the server-side tagging environment when using the server as a Content Delivery Network (CDN).

### Ensuring granular data privacy

When using client-side tagging, the user's browser communicates directly to third parties, which can make it challenging to control the information that is shared. Depending on how your website or app processes user information, there might be a risk of personally identifiable information being shared in HTTP requests.

Server-side tagging gives you full control over the data that is distributed to third parties. Within the server container, you can remove any personally identifiable information (PII) before passing the data on to marketing partners. You can ensure that you are only collecting and sharing data that is necessary and compliant with data privacy regulations.

When you set up your server container to operate in a first-party context, any website data and cookies stay within your domain. This means that vendors can't access third-party cookies. A first-party context allows you to implement tighter content security policies as the browser communicates with fewer or no third-party domains, depending on your setup.

### Improve data quality

In client-side tagging, it is difficult to ensure the consistency and validity of the data as it gets passed directly to the vendor endpoints.

With server-side tagging, you are in control of the data. This allows you to:

-   Correct inconsistencies in event data that may be introduced by different browsers, devices, or other client-side processing
    
-   Reduce the risk of data loss by validating event data to ensure that it meets the criteria necessary to be accepted and processed by the vendor endpoint
    
-   Remove redundant or unnecessary data that may be inserted by the browser or app.
    

## Get started with server-side tagging

Are you ready to learn how to use server-side tagging?

Our learning pathway "Server-side tagging fundamentals" equips you with all the skills you need to get started with server-side tagging. You'll learn how to:

-   Create a tagging server using GCP App Engine
    
-   Set up your tags to send data to your server
    
-   Prepare your servers for live traffic
    
-   Monitor your servers
