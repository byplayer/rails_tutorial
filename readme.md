# What is this?

This repository is named tutorial but this is my rails study logs.

Try to use rails tutorial

[rails tutorial](https://railstutorial.jp/chapters/beginning?version=6.0)

# get start

## set up ruby version

```bash
asdf local ruby 3.1.0
asdf local nodejs 16.14.1
asdf local yarn 1.22.18
```

## setup gem file

```bash
bundle config set path vendor

echo "source 'https://rubygems.org'" >> Gemfile
echo "gem 'bootsnap', require: false" >> Gemfile
echo "gem 'rails', '~> 7.0', '>= 7.0.2.3'" >> Gemfile

bundle install
```

# hello app

## create hello up

```bash
bundle exec rails new hello_app
```

## commit project undr root project

```bash
echo '/vendor/ruby' >> hello_app/.gitignore
rm -rf hello_app/.git

git add .
git commit
```
