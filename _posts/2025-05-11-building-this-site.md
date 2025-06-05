---
layout: post
---

# On building the blog

## Setting the development Environment

1. Install Jekyll
   ```bash
   gem install jekyll bundler
   ```
   
```
ERROR:  Error installing jekyll:
        The last version of ffi (~> 1.0) to support your Ruby & RubyGems was 1.17.2. Try installing it with `gem install ffi -v 1.17.2` and then running the current command again
        ffi requires RubyGems version >= 3.3.22. The current RubyGems version is 3.1.2. Try 'gem update --system' to update RubyGems itself.
Fetching bundler-2.6.8.gem
ERROR:  Error installing bundler:
        The last version of bundler (>= 0) to support your Ruby & RubyGems was 2.4.22. Try installing it with `gem install bundler -v 2.4.22`
        bundler requires Ruby version >= 3.1.0. The current ruby version is 2.7.0.0.
```

I had to update the gems using `sudo gem update`. `gem update --system` didn't work.

The solution was to install a new rube version with `rvm`.
```rvm install 3.2.2```

# Running the site

```
bundle exec jekyll serve --livereload
```


# Theme

https://github.com/poole/hyde