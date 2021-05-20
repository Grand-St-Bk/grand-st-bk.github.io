# Open Streets 
This is a Jekyll site hosted on github pages for (at the time of this writing) Open Streets NYC on Grand St. in Brooklyn NY. CSS handled by Bulma.

## Installation and Development
    $ bundle install
    $ bundle exec jekyll serve --watch

Point your browser to http://localhost:4000

## Deployment
Simply push changes to the remote gh-pages branch.

## Notes
We have used yarn to install bulma. We needed to include the node_modules directory in the repo for github pages to build the css on deployment. The bulma sass files could have been manually added to a sass directory, but to more easily maintain future versions of bulma with yarn, we handled it this way.

We do not recommend adding more much more front-end JS or CSS via yarn as the node_modules directory will likely become unwieldly.