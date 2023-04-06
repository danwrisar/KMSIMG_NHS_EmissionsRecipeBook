#  nhsuk-static-jekyll

<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a href="https://github.com/jekyll">
    <img src="https://github.com/jekyll/brand/blob/master/jekyll-logo-black-red-transparent.png?raw=true" alt="Logo" width="280">
  </a>

  <h3 align="center">Jekyll implementation of the NHS.UK service manual</h3>

  <p align="center">
    <!-- Replace with your repo URL -->
    <a href="https://github.com/craig-shenton/nhsuk-static-jekyll/issues">Report Bug</a>
    ·
    <!-- Replace with your repo URL -->
    <a href="https://github.com/craig-shenton/nhsuk-static-jekyll/issues">Request Feature</a>
  </p>
</p>

<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary><h2 style="display: inline-block">Table of Contents</h2></summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Folder Stucture</a></li>
        <li><a href="#built-with">Built With</a></li>
      </ul>
      <a href="#deploy-to-a-githubio-page">Deploy to a GitHub.io page</a>
    </li>
    <li>
      <a href="#developer-documentation">Developer Documentation</a>
      <ul>
          <li><a href="#getting-started">Getting Started</a></li>
          <li><a href="#verify-your-jekyll-version">Verify your Jekyll version</a></li>
          <li><a href="#fork-then-clone">Fork, then clone</a></li>
          <li><a href="#modify-the-_configyml">Modify the config.yml</a></li>
          <li><a href="#jekyll-serve">Jekyll Serve</a></li>
          <li><a href="#using-github-pages">Using Github Pages</a></li>
          <li><a href="#contact-form">Contact Form</a></li>
          <li><a href="#disqus">Disqus</a></li>
          <li><a href="#customizing-the-css">Customizing the CSS</a></li>
          <li><a href="#page-animation">Page Animation</a></li>
          <li><a href="#anchorjs">AnchorJS</a></li>
          <li><a href="#web-analytics-and-search-engines">Web analytics and search engines</a></li>
      </ul>
    </li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#acknowledgements">Acknowledgements</a></li>
  </ol>
</details>

<!-- ABOUT THE PROJECT -->

## About The Project

This Jekyll theme was originally crafted by [John Otander](http://johnotander.com) as [Pixyll](https://github.com/johno/pixyll), then modified by [Sai Kiran Sripada](https://www.saikiransripada.com/), and then the NHS theme added by [Craig Robert Shenton](https://github.com/craig-shenton). It's free, and open source ([MIT](http://opensource.org/licenses/MIT)).

_**Note:** No NHS data, public or private are shared in this repository._

### Folder Stucture

| Name | Link | Description |
| ---- | --- | ------------ |
| _includes | [[Link](./_includes)] | Element templates |
| _layouts | [[Link](./_layouts )] | Page templates |
| _posts | [[Link](./_posts)] | Blog post markdown files |
| _sass | [[Link](./_sass)] | basscess files |
| assets | [[Link](./assets)] | Image assets |
| css | [[Link](./css)] | css style files |

### Built With

- [Jekyll](https://github.com/jekyll)
- [Liquid](https://shopify.github.io/liquid/)
- [NHS Digital Service Manual](https://service-manual.nhs.uk/)

## Deploy to a GitHub.io page

1. Hit the green 'Use this template' button at the top of this repository page.
2. A new site will open asking you to create a new repository from `nhsuk-static-jekyll`.
3. Give your repository a name. 
4. This is form part of the new website's URL: `https://{github username}.github.io/{repository name}/`.
5. Set the visability to `Public` i.e., Anyone on the internet can see this repository.
6. Hit the green 'Create repository from template' button.
7. GitHub will then clone all the code used to build the website to your new repository.
8. Go to the [_config.yml](https://github.com/craig-shenton/nhsuk-static-jekyll/blob/main/_config.yml) in your new repository.
9. Edit the site settings shown below:

```yml
# ---------------------------------------------------------------------------------------------------------
title:               nhsuk-static-jekyll                  Add a title to your website
email:               craig.shenton@nhs.net                Add your email to the contacts page
author:              Craig Robert Shenton                 Add your name as the defult author for blog posts
description:         "My first website"                   Add sub-text to the 'hero' card on the home page
url:                 "https://craig-shenton.github.io/"   Set to "https://{github_username}.github.io"
baseurl:             "nhsuk-static-jekyll/"               Set this as the same name as your repository
github_username:     craig-shenton                        For adding links to your GitHub page
linkedin_username:   craigrshenton                        For adding links to your LinkedIn page
date_format:         "%b %-d, %Y"                         Sets the date format for the blog pages
# ---------------------------------------------------------------------------------------------------------
```
10. Commit your changes to the repository
11. Go to `Settings > Pages > Source`, change the main branch to `main` and save.
12. GitHub will now deploy your website (~2mins)
13. Go the URL `https://{github username}.github.io/{repository name}/` to view your site.
14. Congratulations! Your website is public [[live example](https://craig-shenton.github.io/nhsuk-static-jekyll/)].

## Developer Documentation

<!-- GETTING STARTED -->

### Getting Started

To get a local copy up and running follow these simple steps.

If you're completely new to Jekyll, I recommend checking out the documentation at <http://jekyllrb.com> or there's a tutorial by [Smashing Magazine](http://www.smashingmagazine.com/2014/08/01/build-blog-jekyll-github-pages/).

```bash
$ git clone git@github.com:craig-shenton/nhsuk-static-jekyll.git
$ cd nhs.pycom
$ gem install bundler 
# If you don't have bundler installed
$ bundle install
```

#### Verify your Jekyll version

It's important to also check your version of Jekyll since this project uses new `baseurl` features that are [only supported in 3.3+](https://jekyllrb.com/news/2016/10/06/jekyll-3-3-is-here/).

### Fork, then clone

Fork the repo, and then clone it so you've got the code locally.


### Modify the `_config.yml`

The `_config.yml` located in the root of the Mixyll directory contains all of the configuration details
for the Jekyll site. The defaults are:

```yml
# Site settings
title: Repo Name
email: your_email@example.com
author: your name
description: "Repo description"
baseurl: ""
url: "http://github-username.github.io"

# Build settings
markdown: kramdown
permalink: pretty
paginate: 3
```

### Jekyll Serve

Then, start the Jekyll Server. I always like to give the `--watch` option so it updates the generated HTML when I make changes.

```bash
$ jekyll serve --watch
```

Now you can navigate to `localhost:4000` in your browser to see the site.

### Using Github Pages

You can host your Jekyll site for free with Github Pages. [Click here](https://pages.github.com/) for more information.

#### A configuration tweak if you're using a gh-pages sub-folder

In addition to your github-username.github.io repo that maps to the root url, you can serve up sites by using a gh-pages branch for other repos so they're available at github-username.github.io/repo-name.

This will require you to modify the `_config.yml` like so:

```yml
# Site settings
title: Repo Name
email: your_email@example.com
author: your name
description: "Repo description"
baseurl: "/repo-name"
url: "http://github-username.github.io"

# Build settings
markdown: kramdown
permalink: pretty
paginate: 3
```

This will ensure that the the correct relative path is constructed for your assets and posts. Also, in order to run the project locally, you will need to specify the blank string for the baseurl: `$ jekyll serve --baseurl ''`.

##### If you don't want the header to link back to the root url

You will also need to tweak the header include `/{{ site.baseurl }}`:

```html
<header class="site-header px2 px-responsive">
  <div class="mt2 wrap">
    <div class="measure">
      <a href="{{ "/" | relative_url }}" class="site-title">{{ site.title }}</a>
      <nav class="site-nav">
        {% include navigation.html %}
      </nav>
    </div>
  </div>
</header>
```

A relevant Jekyll Github Issue: <https://github.com/jekyll/jekyll/issues/332>

### Contact Form

The contact form uses <http://formspree.io>. It will require you to fill the form out and submit it once, before going live, to confirm your email.

More setup instructions and advanced options can be found at [http://formspree.io](http://formspree.io/)

### Disqus

To configure Disqus, set up a [Disqus site](https://disqus.com/admin/create/) with the same name as your site. Then, in `_config.yml`, edit the `disqus_shortname` value to enable Disqus.

### Customizing the CSS

All variables can be found in the `_sass/_variables.scss` file, toggle these as you'd like to change the look and feel of Mixyll.

### Page Animation

If you would like to add a [fade-in-down effect](http://daneden.github.io/animate.css/), you can add `animated: true` to your `_config.yml`.

### AnchorJS

[AnchorJS](https://github.com/bryanbraun/anchorjs): _A JavaScript utility for adding deep anchor links to existing page content. AnchorJS is lightweight, accessible, and has no dependencies._ You can turn it on by toggling `enable_anchorjs`. Because it offers many ways for customization, tweaks should be done in `_includes/footer.html`. Default settings after turning AnchorJS on are:

```html
<script>
    anchors.options.visible = 'always';
    anchors.add('article h2, article h3, article h4, article h5, article h6');
</script>
```

See [documentation](http://bryanbraun.github.io/anchorjs/#basic-usage) for more options.

### Web analytics and search engines

You can measure visits to your website either by using [Google Analytics](https://www.google.com/analytics/) tracking embed or the more advanced [Google Tag Manager](https://www.google.com/analytics/tag-manager/) container.
* For Google Analytics set up the value for `google_analytics`, it should be something like `google_analytics: UA-XXXXXXXX-X`.
* For Google Tag Manager set up the value for `google_tag_manager`, it should be something like: `google_tag_manager: GTM-XXXXX`.
* _Do not_ set both of above methods because this will cause conflicts and skew your reporting data.
* Remember that you need to properly configure the GTM container in its admin panel if you want it to work. More info is available in [GTM's docs](https://www.google.com/analytics/tag-manager/resources/).

Your website is, by default, set to be allowed for crawling and indexing by search engines. (Unless you made yourself a custom robots.txt file). You can use front matter settings on each page to control how search engines will it. Sometimes you may want to exclude a particular page from indexing or forbid Google to store a copy of your page in its cache. It is up to you. Use the `meta_robots` frontmatter key and assign values based on [this table](https://developers.google.com/webmasters/control-crawl-index/docs/robots_meta_tag?hl=en#valid-indexing--serving-directives). Some examples:

```yaml
# exclude page from index
meta_robots: noindex

# allow indexing, disallow caching
meta_robots: noarchive

# allow indexing, disallow crawling links
meta_robots: nofollow

# disallow indexing, follow links
meta_robots: noindex,follow
```

In order to get more information about your website's status in search engines, you can register it in [Google Search Console](https://www.google.com/webmasters/tools/home) and/or [Bing Webmaster Tools](http://www.bing.com/toolbox/webmaster). Both these tools will ask you to authorize your website with them and there are couple of ways to do that. Mixyll supports verification via meta tags - just fill in values for `google_verification` and/or `bing_verification` in `_config.yml`, the verification strings and meta tags will then be added automatically.

If search engine optimization is your thing, you can also set up `meta_description` values for each page/post. By default Mixyll uses `summary` to populate the `<meta name="description" content="...">` tag and falls back to `description` from `_config.yml` if `summary` is not present in page/post's front matter. The `summary` is also used for generating Open Graph tags. Why would you want to use a dedicated variable for meta description? Because character limit to properly display this description in search results (as a snippet) is way smaller than in Open Graph. It is recommended to keep it at 155-160 characters, for more in-depth info read [this article](https://moz.com/blog/i-cant-drive-155-meta-descriptions-in-2015).

And lastly - if you happen to write in language other than English be sure to change `og_locale` in `_config.yml` to reflect it.


#### Ensure there's an upstream remote

If `git remote -v` doesn't have an upstream listed, you can do the following to add it:

```
git remote add upstream https://github.com/{{ site.github_username }}/{{ site.baseurl }}.git
```

#### Pull in the latest changes

```
git pull upstream master
```

There may be merge conflicts, so be sure to fix the files that git lists if they occur. That's it!

<!-- CONTRIBUTING-->

## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

_See [CONTRIBUTING.md](./CONTRIBUTING.md) for detailed guidance._

<!-- LICENSE -->

## License

Distributed under the MIT License. _See [LICENSE.md](./LICENSE) for more information._

<!-- ACKNOWLEDGEMENTS -->
## Acknowledgements

* Splash Photo by <a class="nhsuk-footer__list-item-link" href="https://unsplash.com/@cdr6934?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Chris Ried</a>
