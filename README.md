# GitHub Pages Bootstrap

- Jekyll-based site for GitHub Pages
- Bootstrap front-end framework

## Ruby Dev Environment: Linux
- Install `rbenv` by cloning the GitHub repo
- Set rbenv to `v1.1.2` via git
- Install `ruby-build` as a rbenv plugin
- Set ruby-build to `v20200214` via git

Add rbenv to your local PATH (bash shell):
```
$ echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bash_profile
```

Set up rbenv in your shell:
```
$ ~/.rbenv/bin/rbenv init
```
Follow the printed instructions to set up rbenv shell integration.

Restart your shell so that PATH changes take effect.
On Linux, log out and then log back in.

Check your local Ruby environment with this command:
```
$ curl -fsSL https://github.com/rbenv/rbenv-installer/raw/master/bin/rbenv-doctor | bash
```

Install Ruby 2.6.5:
```
$ rbenv install 2.6.5
```

Set global Ruby version:
```
$ rbenv global 2.6.5
```

Check local gem environment:
```
$ gem env home
```
This should return the path to rbenv in `USER_HOME/.rbenv/versions/...`

Install bundler:
```
$ gem install bundler
```

Install missing gem packages:

```
$ bundle install
```

Update gem packages if desired:

```
$ bundle update
```

Build site and launch Jekyll server:

```
$ bundle exec jekyll serve
```

The development site will load at
[http://localhost:4000/gh-pages-bootstrap/](http://localhost:4000/gh-pages-bootstrap/).
