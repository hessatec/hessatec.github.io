# Hessatec Site

![Hessatec logo.](logo.png)

## Introduction

This repository houses the hessatec.com site source code, which is served through Jekyll and GitHub Pages. You can find a more comprehensive overview of the Jekyll directory structure [here.](https://jekyllrb.com/docs/structure/) To get started, here are the key directories to consider:

1. `/_includes/` -- this folder contains structures common to each page, like the navigation bar and the page footer.
2. `/_layouts/` -- this folder includes the templates that define the structure for certain pages. There are currently two layouts defined -- one for standard site pages (`default.html`) and one for blog posts (`post.html`).
3. `/_posts/` -- this is the primary reason we opted for the more complex Jekyll-based solution. The flexibility it provides for blogging. Most likely, you do not need to touch the content of these posts, especially not the file name (Jekyll requires these file names to follow a convention).
4. `/_sass/` -- this directory contains the SASS partials. Standard CSS code is compatible with SASS, however SASS defines extensions to CSS. We have used very few of the features provided by SASS, other than it allows us to separate our CSS classes into multiple files. Then, one file, `assets/css/styles.scss`, uses directives to import these partials.
5. HTML or Markdown files -- these are the actual contents of our site's pages (besides the blog posts). The HTML code is injected into the `{{ content }}` tags in the layouts folder (see #2).

## Running the Site Locally

Here are the steps to follow to set up Jekyll locally on your machine:

1. Install Jekyll and its dependencies (https://jekyllrb.com/docs/installation/)
2. Type `bundle exec jekyll serve` in a terminal located in the root path of this repository. A `/_site/` folder will be generated if you wish to inspect the code that Jekyll has produced.

## Improvements

The initial site design does not meet our requirements. In summary, here is what we need improved:

- We have created wireframes. The site needs to be updated in accordance with these wireframes. We will provide these wireframes. 
- [Here are the results of a free SEO audit.](https://seositecheckup.com/seo-audit/hessatec.com) Some of these recommendations are very easy to implement, but they may make a difference to our site and brand recognition. This list is not comprehensive.
- Analytics integration. The most popular service is Google Analytics. We'd like to understand what demographics are accessing our site and the characteristics about their session (e.g. time spent on each page).

## Contributing

The site is currently served from the `main` branch. Please create another branch and open a pull request for each feature implemented. Assign me (`saimachi`) as a reviewer.
