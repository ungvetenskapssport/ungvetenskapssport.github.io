# Ung Vetenskapssport

Soon this will be our official website, built with jekyll using project-pages theme. 

This website runs jekyll which is written in ruby, installation for ubuntu:

Install on macos:
- install [brew](https://brew.sh/)
- install jekyll: `brew install jekyll`

Install on ubuntu:
- `sudo apt-get install ruby-full build-essential zlib1g-dev`
- `gem install jekyll bundler`

Run local webserver with `make dev`

Install on Windows:
There are some kinks to work out here, but it is possible. Worked on Windows 11 2023-03-26.
- Install Ruby
- Initiate a gemfile "$ bundle init" in the ...github.io-repo
- Remove all the random new files except "Gemfile"
- Update the gemfile to add github-pages package: "gem 'github-pages', group: :jekyll_plugins"
- Change the Jekyll version to 3.9.0 (from >4 something...) in the ruby-file
- Re-install all the dependencies
- Add "$ bundle add webrick"

- run `$ bundle exec jekyll serve` when you want to run the site locally
- Go to the specified address in your browser.
