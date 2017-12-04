# Feathercoin Site

## Basic Text Edits
This is the new build of the Feathercoin site built on Bootstrap 4.0 and Jekyll.  Jekyll was chosen because site updates to text can happen through a Github commit, making it possible to collaborate and make changes quickly.  To make changes to text on the website, in the root directory you will find .md files (index.md, about.md etc) each coorespond with their own page.  Just checkout the page, make the changes and push the commit to GitHub and you are done!  Easy peezy.

## Changing the templates
To get started with local development you will need to follow the steps found here: https://jekyllrb.com/.  The structure of the Jekyll site is very simple and outlined below:

* _includes folder - These are small bits of code that are called on our _layouts making it possible to reuse code across the website.  For example, the header is in the includes folder and each layout references that same header so there is no duplication of code
* _layouts folder - This is the template for the each page.  You will find in each markdown file (i.e. index.md) that the top of the page calls which layout to use, then each of the fields below that dictate what will show up in each part of the template.  It makes it very simple to create new pages since you can create a new markdown file, reference the template and start filling in each variable with what you would like
* _site folder - This is the final built site that Jekyll generates after build that is published.  Do not edit any files here as they get overwritten each time Jekyll builds your site with your latest changes
* assets folder - This is where any assets that the website is using are stored
* markdown files - These represent the individual pages on the website where you change the text next to their cooresponding variables for display on the page.

## A Few "Gotchyas"

1. If a page errors out in Jekyll nothing will be displayed.  Common problems are using returns when specifying a varible for example:
##Wrong
headermessage: Look at what I've done
Thing 1
Thing 2
Thing 3
##Right
headermessage: Look at what I've done <br> Thing 1 <br> Thing 2 <br> Thing 3

2. If you use a colon in your text it will error out.  Instead, either use a different character or use &#58; to display a colon.

Looking forward to seeing what the community can do with this as a base!
