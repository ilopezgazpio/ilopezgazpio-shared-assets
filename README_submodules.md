# Shared assets for drone websites


## Manual Update in Each Secondary Repo

1. Navigate to secondary repo
2. git submodule update --remote --merge


## Initialize submodule

git submodule add git@github.com:ilopezgazpio/drone-shared-assets.git shared


## Remove submodule

git submodule deinit -f assets


## If cloning for the first time, run

git clone --recurse-submodules https://github.com/your-username/secondary-repo.git


## To initialize a submodule, run

git submodule init
git submodule update


## Local Deployment of site (and debugging :S )

- apt requirements

```
ruby-dev header files
ruby-bundler
jekyll
jekyll github
```

- create a Gemfile with the content

```
source "https://rubygems.org"

gem "github-pages", group: :jekyll_plugins
gem "webrick"
```

then run

```
bundle install
```

- bundle requirements

```
jekyll - gem install bundler jekyll
```

For deployment, run:

```
ruby -v
jekyll -v
bundle exec jekyll serve --port 4000
```
