# rssfeed
Simple RSS feed generator based on Jekyll

* Creates a `feed.xml` file and an (optional) HTML directory of posts to be transplanted into a static website.
* Posts can be Markdown or HTML.
* Atom 1.0 compliant feed.

## Usage

1. I recommend forking the project and using it as a base in order to further configure the Atom file and feed HTML directory beyond the configuration file.
2. Get Jekyll and Bundler `gem install bundler jekyll`.
3. Install gems `bundle install`.
4. Configure the site and run `bundle exec jekyll build`.
5. Transplant the files within `_site` into your static website.

## Guide

*Post creation and further configuration is coming.*

## Site configuration

Configuration variables to be changed in `_config.yml`.

|Name|Description|
|-|-|
|`title`|Title of the overall website, not the feed portion specifically.|
|`author`|Name of the author.|
|`email`|Email of the author.|
|`description`|Feed's description.|
|`baseurl`|Configure if not transplanting generated files directly into the root of the website. Must contain a trailing `/`.|
|`url`|URL of the overall website without a sub-directory and without a trailing `/`.|
|`home_url`|Relative URL to the homepage of the website, e.g. `/`.|
|`home_display`|Vanity display name to the homepage of the website, e.g. "Homepage".|

## Post configuration

Variables that sit above a post.

|Name|Description|
|-|-|
|`title`|Title of the post.
|`date`|ISO 8601 date.|
|`date_display`|Date displayed on the feed website in any date format.|
|`layout`|Jekyll layout to use, usually kept as default but is required.|
|`categories`|The sub-directory to place the post in, e.g. `feed`.|