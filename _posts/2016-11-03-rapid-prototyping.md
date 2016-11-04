---
layout: post
title:  "Rapid Prototyping"
date:   03-11-2016 00:43:32
categories: code
---

## Thoughts

<br>

## Done

* Fixed timestamp issue in Jekyll date: field
* Created new git repo for <code>findscribe</code>

<br>

## Rosalind.info

* Hilarious amount of attempts to find out out that INI2 just wanted the "number" returned, not the code...

<br>

## Rails
rails new findscribe
added to Gemfile:   gem 'rspec-rails', '2.14.1'
added to Gemfile:

```ruby
group :test do
  gem 'selenium-webdriver', '2.35.1'
  gem 'capybara', '2.1.0'
end

group :production do
  gem 'pg', '0.15.1'
  gem 'rails_12factor', '0.0.2'
end
```
<br>
