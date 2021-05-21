# Open Streets 
This is a Jekyll site hosted on github pages for (at the time of this writing) Open Streets NYC on Grand St. in Brooklyn NY. CSS handled by Bulma.

## Installation and Development
Request access to the Grand St. Brooklyn github organization.

### Requirements
This requires **ruby 3.0.1** (for no reason other than it being the latest stable version at the time of this writing:). To install a specific version of ruby, we recommend that you use a ruby version manager such as [rbenv](https://github.com/rbenv/rbenv) (easiest) or [rvm](https://rvm.io/).

### Installation
With the appropriate version of ruby installed grab the code and switch to the gh-pages branch.

    $ git clone [repository url]
    $ git checkout gh-pages
    $ bundle install
    $ bundle exec jekyll serve --watch

Point your browser to http://localhost:4000. Jekyll will render a local static version of the site in \_site and 

## Deployment
Simply push changes to the remote gh-pages branch.

## Notes
We have used yarn to install bulma. We needed to include the node_modules directory in the repo for github pages to build the css on deployment. The bulma sass files could have been manually added to a sass directory, but to more easily maintain future versions of bulma with yarn, we handled it this way.

We do not recommend adding more much more front-end JS or CSS via yarn as the node_modules directory will likely become unwieldly.