
In this gh-pages you find the proposition for a HomePage for the GnuBee Personal Cloud.

See https://pages.github.com/ for what gh-pages can be used for.


Additionally to make the live of the developer/maintainer of this home page easier,
I add a Gemfile and a Rakefile which can be used (assuming you have ruby installed) to
make it easy to start a local webserver. If you started (as described below) you can 
afterwards point your browser at http://127.0.0.1:4000. You should see a preview of the
actual content. As soon as you save changes in a file, the webserver will reload the content


To start the webserver you
* gem install bundler
* bundle install
* bundle exec rake webserver

The first two comands must only be called once.

Once you are satisfied, commit your changes and push them to github. 

Enable the gh-pages in your repository settings, e.g.
https://github.com/<yourname>/GnuBee_Docs/settings

After pushing the changes and waiting for a few seconds or minutes
you should be able to point your browser at https://<yourname>.github.io/GnuBee_Docs/.
