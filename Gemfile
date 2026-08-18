source "https://rubygems.org"

# Pins Jekyll and its plugins to the versions GitHub Pages runs, so local
# builds match the deployed site. Plugins are enabled in _config.yml and ship
# as dependencies of this gem, so they are not listed separately.
gem "github-pages", group: :jekyll_plugins

group :jekyll_plugins do
  gem "webrick", "~> 1.8" # no longer bundled with Ruby 3.0+
end

gem "wdm", "~> 0.2" if Gem.win_platform? # filesystem watching on Windows

# Windows has no system timezone database; Linux, which GitHub Pages runs, does.
gem "tzinfo-data", platforms: [:mingw, :x64_mingw, :mswin, :jruby]
