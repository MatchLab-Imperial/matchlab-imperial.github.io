[![Netlify Status](https://api.netlify.com/api/v1/badges/8c17197c-9282-49f1-a779-d0409b3da2c6/deploy-status)](https://app.netlify.com/sites/flamboyant-darwin-3ada19/deploys)

Jekyll site for Matchlab.

# Dev branch
- Runs at http://localhost:4000
- To run use:
  - `bundle install`
  - `jekyll serve`

## Site navigation
Manage site wide navigation from `_data/site_nav.yml`. Every entry represents a menu item with its name and URL it points to. The URL can be a relative link like `/research` or a URL like 'https://example.com'. Make sure to use 'http:// or https://' for web links

## Updating baseURL
- update `url` key in `_config.yml` to the site URL.