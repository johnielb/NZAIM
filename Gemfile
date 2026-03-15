source "https://rubygems.org"

gem "jekyll", "~> 4.3"

# No gem-based theme — custom theme only
# Required Jekyll plugins
group :jekyll_plugins do
  gem "jekyll-feed"
  gem "jekyll-seo-tag"
end

# Platform fixes
platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end

gem "wdm", "~> 0.1", platforms: [:mingw, :x64_mingw, :mswin]
gem "http_parser.rb", "~> 0.6.0", platforms: [:jruby]
