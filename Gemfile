# use `bundle exec jekyll serve -l -P 3000` locally to test out site on port 3000
#      default port is 4000. `-l` is livereload
# create new blogs in _posts named by date-title.md

# NOTE: Jekyll requires front matter (triple dash yaml section) to the top of all
#       markdown files. But it can be empty. Files inside `_posts` directory are
#       special and don't even require the empty front section for some reason.

# example code syntax highlighting
# ```elixir
#   defp http_req(req, options) do
#     options
#     |> Enum.into(req)
#     |> MyGateway.perform()
#   end
# ```

# general help url
# https://help.github.com/en/categories/customizing-github-pages

source 'https://rubygems.org'

gem 'jekyll'

group :jekyll_plugins do
  gem 'jekyll-sitemap'
  gem 'jekyll-feed'
  gem 'jekyll-seo-tag'
  gem "github-pages"
end
