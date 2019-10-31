pokemon5e.com

Based on the theme by the [SinglePaged Jekyll Theme](Fancy jekyll)

# Contributing
## Fork the project repo

## Install in your local development environment
We want to test our changes locally for this we will be using [Ruby](https://jekyllrb.com/docs/installation/).

Once you've found a home for your forked repository, **[clone it](https://help.github.com/articles/cloning-a-repository/)**.

### Install Jekyll

Jekyll is a [Ruby Gem](https://jekyllrb.com/docs/ruby-101/#gems) that can be installed on most systems.

1. Install a full [Ruby development environment](https://jekyllrb.com/docs/installation/)
2. Install Jekyll and [bundler](https://jekyllrb.com/docs/ruby-101/#bundler) [gems](https://jekyllrb.com/docs/ruby-101/#gems)
```
gem install jekyll bundler
```
3. Change into your new directory
```
cd pokemon5e.github.io
```
4. Install missing gems
```
bundle install
```
5. Build the site and make it available on a local server
```
bundle exec jekyll serve
```

You should see something like:

```
Configuration file: /octocat/pokemon5e.github.io/_config.yml
            Source: /pokemon5e.github.io
       Destination: pokemon5e.github.io/_site
 Incremental build: disabled. Enable with --incremental
      Generating...
   GitHub Metadata: No GitHub API authentication could be found. Some fields may be missing or have incorrect data.
                    done in 2.729 seconds.
 Auto-regeneration: enabled for '/pokemon5e.github.io'
    Server address: http://127.0.0.1:4000
  Server running... press ctrl-c to stop.
```


Don't worry about the "No GitHub API authentication could be found" message.  We are not using much of the Github API.

6. Now browse to [http://localhost:4000](http://localhost:4000)

## Editing the Website

#### Colors
Changes to predefined colors are made in `_config.yml` that will then get inserted into auto generated CSS files. Remember that to see changes in this file you need to restart the local server, press ctrl-c to stop and then `bundle exec jekyll serve` to start it again.

#### Adding Resource
Before you add a resource you need a banner, I have the "source" templates of the banners located within `/pokemon5e.github.io/_source/`. Save it out as a png in `/pokemon5e.github.io/img/`.

You add it to the website by editing the file `/pokemon5e.github.io/_data/resources.json`, create a new list entry and insert image, description (don't forget the authors name!) and the url.