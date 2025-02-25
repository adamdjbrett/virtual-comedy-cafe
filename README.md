# To do
  - update `scss` language
  - do I need thumbnail on the homepage or can I just go with coverImage?
    - switched homepage to coverImage and removed thumbnail lets see what happens

[![Netlify Status](https://api.netlify.com/api/v1/badges/bbf28a84-4bdb-407b-a2fa-32628d27fa3d/deploy-status)](https://app.netlify.com/sites/eleventy-netlify-boilerplate/deploys)

# Eleventy Netlify Boilerplate

## What is it?

A simple template for building a fast, static website using the [Eleventy](https://www.11ty.io/) static site generator, with [Netlify CMS](https://www.netlifycms.org/) baked-in, ready to deploy to [Netlify](https://www.netlify.com) in a couple of clicks.

Use it as a starter for your own projects or as an easy way to get started building websites with Eleventy.

Based on the [Eleventy Base Blog](https://github.com/11ty/eleventy-base-blog) repo (see there for additional info on Eleventy usage).

🔥 **This project is featured on Netlify's official [template showcase](https://templates.netlify.com/template/eleventy-netlify-boilerplate/) and blog: [The top 10 Static Site Generators to watch in 2018](https://templates.netlify.com/template/eleventy-netlify-boilerplate/)** 🔥

## [Demo Site](https://eleventy-netlify-boilerplate.netlify.com//)

## Features

* Sample pages and blog with tag support
* Netlify CMS with editor previews (thanks [@biilmann](https://github.com/biilmann)!)
* CSS 2kb minified, inlined for fastest page render
* Pre-builds and minifies your HTML
* Responsive CSS Grid layout, with fallbacks (see [Browser Support](#browser-support))
* Uses Markdown files for content
* Uses Liquid and/or Nunjucks templates for layout
* 100% Javascript framework free
* Optional pipeline for minified inline JS
* Continuous Deployment workflow via Netlify

## Want to try it out now?

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/danurbanowicz/eleventy-netlify-boilerplate&stack=cms)

Clicking the button above will deploy a copy of the demo website to your Netlify
account (you can create an account during this process if you don't have one)
and everything needed for running the CMS:

* A new repository in your GitHub account with the code
* Full Continuous Deployment to Netlify's global CDN network
* Control users and access with Netlify Identity
* Manage content with Netlify CMS
* Process form data with Netlify Forms

### Setup authentication

After deploying this project, Netlify Identity will add you as a CMS user and
will email you an invite. It is not necessary to accept this invite if you wish
to use an
[OAuth provider](https://www.netlify.com/docs/identity/#external-provider-login)
(e.g. Github) to manage authentication for your CMS.
It is recommended to use this method of authentication as it removes the need
for an email & password to log in to the CMS and is generally more secure. You
will need to add an OAuth provider in your Netlify app settings under
"Settings" > "Identity" > "External providers".

Once you've added an OAuth provider, navigate to `/admin` on your site, select your provider from the
list, and you should then be logged into your CMS. Cool huh?

Now you're all set, and you can start editing content!

## Gotchas

If you change the repo that was created at deploy time from public to private, you'll need to regenerate your token,
as the token generated using the deploy to Netlify button can only access public repositories. To
regenerate your token, head to "Settings" in your Netlify site dashboard, go to the "Identity"
section, then scroll to "Services" where you'll see an "Edit settings" button. Click that and you'll
see a text link to "Generate access token in GitHub".

If you need any help with setting up Netlify CMS, you can reach out to the Netlify team in the [Netlify CMS Gitter](https://gitter.im/netlify/netlifycms).

## Local development

### 1. Clone this repository:

```
git clone https://github.com/danurbanowicz/eleventy-netlify-boilerplate.git my-blog-name
```


### 2. Navigate to the directory

```
cd my-blog-name
```

Specifically have a look at `.eleventy.js` to see if you want to configure any Eleventy options differently.

### 3. Install dependencies

```
npm install
```

### 4. Edit _data/metadata.json

This file contains your site title and author details.

### 5. Run Eleventy (builds the site)

```
npx eleventy
```

Or build automatically when a template changes:
```
npx eleventy --watch
```

Or in debug mode:
```
DEBUG=* npx eleventy
```

## Bug reports, feature requests, etc

This is an ongoing project and I welcome any feedback, suggestions or contributions.

Please use the issue tracker to let me know about any bugs or feature requests, or alternatively make a pull request.

If you need any help with setting up Netlify CMS, you can reach out to the Netlify team in the [Netlify CMS Gitter](https://gitter.im/netlify/netlifycms).

## [Browser support](#browser-support)

This template uses relatively new features such as [CSS Grid layout](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Grid_Layout) and [CSS Custom Properties](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Variables) therefore you should probably consider providing fallbacks for older or less capable browsers before using this template in a production environment.
