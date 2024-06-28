---
layout: blog-post

title:  "Step-by-Step Guide: Installing Jekyll and Hosting Your Site on GitHub Pages"
date:   2023-10-12 17:35:09 +0600
categories: [Code, Jekyll, github pages]
keywords: Health  Travel Life Style
description: Have you ever wanted to create a simple and elegant website or blog without the complexities of traditional content management systems? Jekyll is the answer
image: "https://tds-images.thedailystar.net/sites/default/files/styles/big_202/public/images/2023/10/10/importance_of_independent_judiciary.jpg"

team:
  name: Lukas Devlin
  subtitle: Digital Marketer and Social Media Manager
# other front matter fields
  username: lukas_devlin
  tag: Chief Editor / Blogger
  permalink: lukas-devlin
  date: 2023-10-12 17:35:09 +0600
  message: |
      There live the blind texts. Separated they live in Bookmarksgrove right at the coast of the Semantics, a large language ocean.
  image: /assets/images/person_3.jpg
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

### Step-by-Step Guide: Installing Jekyll and Hosting Your Site on GitHub Pages

In this guide, we'll walk you through the process of installing Jekyll, a static site generator, and hosting your site on GitHub Pages.

#### Prerequisites

Before you begin, make sure you have the following prerequisites:

- A GitHub account (if you don't have one, sign up at [GitHub](https://github.com/))
- Basic knowledge of Markdown and HTML
- Ruby installed on your computer (if not, install it from [Ruby's official website](https://www.ruby-lang.org/en/documentation/installation/))
- Basic knowledge of the command line (Terminal or Command Prompt)

#### Step 1: Install Jekyll

1. Open your command line interface.

2. Install Jekyll by running the following command:

```
//shell{1}
gem install bundler jekyll
```

1. Verify the installation by running:

```
//shell{1}
jekyll -v
```

You should see the installed Jekyll version.

Step 2: Create a Jekyll Site
1. Create a new Jekyll site by running:

```
//shell{1}
jekyll new my-site
```
Replace "my-site" with your desired site name.

1. Change to the site directory:

```
//shell{1}
cd my-site
```

Step 3: Preview Your Site Locally
1. Start a local development server:

```
//shell{1}
bundle exec jekyll serve
```

1. Open a web browser and navigate to http://localhost:4000 to preview your site.
Step 4: Customize Your Site

2. Customize your site by editing the files in the _layouts, _includes, and _posts directories.

3. Explore the _config.yml file to configure site settings.

Step 5: Create a GitHub Repository

1. Go to GitHub and log in to your account.

2. Click the "+" button in the top right corner and select "New repository."

3. Name your repository. For a GitHub Pages site, the repository name should be in the format username.github.io, where "username" is your GitHub username.

4. Choose the repository's visibility (public or private) and initialize it with a README file.

5. Click "Create repository."

Step 6: Publish Your Site
1. Push your Jekyll site to the GitHub repository:
```
//shell{1}
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/username/username.github.io.git
git push -u origin main
```

Replace "username" with your GitHub username.

1. Wait a few moments for GitHub to build your site. Your site will be available at https://username.github.io.
Step 7: Customize Your Domain (Optional)
1. If you have a custom domain, follow GitHub's guide to configure it for your GitHub Pages site.
Step 8: Update Your Site
1. Edit your Jekyll site locally.

2. Push your changes to GitHub to update your live site.

Congratulations! You've successfully installed Jekyll and hosted your site on GitHub Pages. Your site is now accessible to the world.

```
//csharp
You can copy and paste this entire Markdown code, including the formatted code blocks with line numbers, into your Markdown file.
```