# Think Feel Do So Features

## Add as a dependency and load rake tasks

In the `Gemfile` add

    gem 'think_feel_do_so_features',
        git: 'https://github.com/cbitstech/think_feel_do_so_features.git'

Install the gem

    bundle install

In the `Rakefile` add

    spec = Gem::Specification.find_by_name 'think_feel_do_so_features'
    load "#{ spec.gem_dir }/lib/tasks/load_fixtures.rake"

Load the fixtures

    $ bin/rake load_fixtures
