pry-rails Subvisual fork
========================

This fork of [rweng/pry-rails] was created to keep a trustworthy and stable
source for the `pry-rails` gem with the patch proposed in [rweng/pry-rails#112].
This patch limits loading `pry` to the Rails console, consequently reducing the
initial bundle memory footprint by over 6MB. This makes it viable to use [Pry]
as the Rails console even in production.

The base version of this fork is [v0.3.9].


Installation
------------

Add this line to your application's Gemfile:

```ruby
gem "pry-rails", git: "https://github.com/subvisual/pry-rails.git"
```

And then execute:

    $ bundle install

Or install it yourself as:

    $ gem install pry-rails


### Using pry outside of Rails console

If you want to use [Pry] outside of Rails console, you have to add it to your
application's Gemfile explicitly:

```ruby
gem "pry", group: :development
```


Usage
-----

This gem makes [Pry] available only for the Rails console.

    $ rails console


Development
-----------

Please contribute to rweng/pry-rails and let us know so we can rebase from
there. If your contribution is not accepted or is ignored, feel free to [open
a pull request here].


Contributing
------------

Please prioritize contributing to [rweng/pry-rails] and let us know so we can
rebase from there.

If your contribution is not accepted, or is ignored, feel free to open
a pull request on GitHub at https://github.com/subvisual/pry-rails.

Bug reports specific to this fork are always welcome and appreciated.


License
-------

pry-rails is copyright &copy; 2012 Robin Wenglewski

pry-rails Subvisual fork is a modification of pry-rails. It includes a notable
contribution by Kelly Stannard, proposed to the original project in
[rweng/pry-rails#112].

pry-rails Subvisual fork is open-source, made available for free, and subject
to the same terms of [rweng/pry-rails] as reflected in its [license].


About
-----

This fork of pry-rails is maintained with :heart: by [Subvisual][subvisual].

[![Subvisual][subvisual-logo]][subvisual]


[rweng/pry-rails]: https://github.com/rweng/pry-rails
[rweng/pry-rails#112]: https://github.com/rweng/pry-rails/pull/112
[Pry]: https://github.com/pry/pry
[v0.3.9]: https://github.com/rweng/pry-rails/tree/v0.3.9
[license]: ./LICENSE.txt
[rubygems.org]: https://rubygems.org
[subvisual]: http://subvisual.com
[subvisual-logo]: https://raw.githubusercontent.com/subvisual/guides/master/github/templates/logos/blue.png

