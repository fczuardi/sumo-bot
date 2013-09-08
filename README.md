Commands
--------
.os - Get information about the OS the bot is running on.
.stats - Get information about the running bot process.
.version - Get Node version information.
.listfeeds - Get a list of all the feeds in the config.
.feedinfo (feedname) - Get information on the specified feed.

Running on Heroku
-----------------

After pushing to your heroku git:

### Start

    $ mv Gimfile Gemfile
    $ bundle exec heroku ps:scale worker=1

### Stop
    $ bundle exec heroku ps:scale worker=0
    $ mv Gemfile Gimfile
