# Changelog

### v1.4

**This release requires Hugo v0.53 or greater**

- Highlight.js has been replaced by Chroma (Hugo's built-in syntax highlighter)
- Content on the homepage is only displayed if it's in `.Site.Params.mainSections`
- Related content will be listed at the bottom of a blog post
- Taxonomy terms like tags and categories displayed on their own page, i.e. `/tags/hugo`
- The Google Analytics template has been wrapped in the `tracking.html` partial to ease an override
- Upgrade Fontawesome to 5.8.0
- The header image on the homepage can now be used without a header text
- Add support for an apple-touch-icon
- Add Speakerdeck icon

### v1.3

**This release requires Hugo v0.19 or greater** due to the deprecation of the `.Now` attribute.

Furthermore, the `exampleSite` folder has become a standalone demo by modified the `themesDir` property in the `config.toml`. Make sure to comment out `themesDir` in the config file if you use the theme in production. [Read more](/README.md#setup)

The addition of the `disableComments` variable in the frontmatter the comment section can be disabled on individual pages.


### v1.2

- Update hightlight.js and fontawesome
- Add Gitlab and Trello icon

### v1.1

**This release requires Hugo v0.16 or greater**. The Gravatar image required the manual creation
of an MD5 hash in order to generate an avatar. Now, this is done automatically. The avatar still
depends on the `gravatar` variable in the config file.
