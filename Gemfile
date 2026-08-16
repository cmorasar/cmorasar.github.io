source "https://rubygems.org"

# The github-pages gem pins Jekyll and the plugin set to exactly what
# GitHub Pages runs in production, so a local build matches the deployed site.
# Run Jekyll through Bundler so this version is the one used:
#
#     bundle exec jekyll serve --config _config.yml,_config.dev.yml
#
gem "github-pages", group: :jekyll_plugins

# Which plugins are actually enabled is controlled by `plugins:` in _config.yml.
# They ship as dependencies of github-pages, so they are not repeated here.

group :jekyll_plugins do
  gem "webrick", "~> 1.8" # no longer bundled with Ruby 3.0+
end

# Windows-only: lets Jekyll watch the filesystem for changes.
gem "wdm", "~> 0.2" if Gem.win_platform?
