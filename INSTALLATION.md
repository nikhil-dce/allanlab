INSTALLATION

# Allan Lab Website

This is the website of our academic research group at Leiden University.

This website is powered by Jekyll and some Bootstrap, Bootwatch. We tried to make it simple yet adaptable, so that it is easy for you to re-use it for your purpose. Plese feel free to copy and modify for your own purposes.  You don't have to link to us or mention us (but of course we appreciate it).

Go to *aboutwebsite.md*  to learn how to copy and modidy this page for your purpose. 


Copyright Allan Lab. Code released under the MIT License.



# SPARk Lab
Hi, everyone

So, we need to install ruby, jekyll


## Install Ruby

Install ruby

tutorial from - https://gorails.com/setup/ubuntu/14.10

Install dependencies 
```
sudo apt-get update
sudo apt-get install git-core curl zlib1g-dev build-essential libssl-dev libreadline-dev libyaml-dev libsqlite3-dev sqlite3 libxml2-dev libxslt1-dev libcurl4-openssl-dev python-software-properties libffi-dev
```

Install rbenv, which is a package manager for installing ruby

```
cd
git clone https://github.com/rbenv/rbenv.git ~/.rbenv
echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bashrc
echo 'eval "$(rbenv init -)"' >> ~/.bashrc
exec $SHELL

git clone https://github.com/rbenv/ruby-build.git ~/.rbenv/plugins/ruby-build
echo 'export PATH="$HOME/.rbenv/plugins/ruby-build/bin:$PATH"' >> ~/.bashrc
exec $SHELL

rbenv install 2.3.1
rbenv global 2.3.1
ruby -v
```



## RUBY GEMS
gems is basically package manager for ruby. Like pip is for python.
so update gems

```
gem update --system
```

## INSTALL NODEJS

Install nvm

tutorial from - http://www.hostingadvice.com/how-to/install-nodejs-ubuntu-14-04/#node-version-manager

```
curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.31.0/install.sh | bash

nvm install 6.9.1
nvm use 6.9.1
```

## JEKYLL


```
gem install bundler
gem install jekyll
```

#######################
DONE

A basic Jekyll site usually looks something like this:
```
.
├── _config.yml
├── _drafts
|   ├── begin-with-the-crazy-ideas.md
|   └── on-simplicity-in-technology.md
├── _includes
|   ├── footer.html
|   └── header.html
├── _layouts
|   ├── default.html
|   └── post.html
├── _posts
|   ├── 2007-10-29-why-every-programmer-should-play-nethack.md
|   └── 2009-04-26-barcamp-boston-4-roundup.md
├── _data
|   └── members.yml
├── _site
├── .jekyll-metadata
└── index.html
```
# Now COPY THE REPO
```
git https://github.com/ankitp94/lab-website.git
cd lab-website
bundle install
```
# Confirm that its working
```
bundle exec jekyll -v
bundle exec jekyll serve
```
AND
visit the following address to see the live website.
```
 http://127.0.0.1:4000/
```

DONE


Start making changes.
