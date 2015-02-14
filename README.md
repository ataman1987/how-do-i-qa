# How do I QA?
Introduction to acceptance testing


# Database setup

We're using postgres.

`sudo -u postgres psql template1`

**Fill in your desired password** in the `db/development_setup_script.sql` - if you leave it empty you might have to [change your hba_conf](https://gist.github.com/p1nox/4953113).

Then in the pql console run: `\i /path/to/db/development_setup_script.sql`
Exit console by typing `\q`

**Copy database.yml.sample to database.yml and fill in the password you chose earlier.**

Then `rake db:reseed` to populate development environment with example data.

# Gem dependencies

[Webkit as js driver for cabypara](https://github.com/thoughtbot/capybara-webkit/wiki/Installing-Qt-and-compiling-capybara-webkit)

# Run

`rails s`
