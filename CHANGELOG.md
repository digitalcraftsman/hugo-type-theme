# Changelog

### 1st April 2017

**This change requires Hugo v0.19 or greater** due to the deprecation of the `.Now` attribute.

Furthermore, the `exampleSite` folder has become a standalone demo by modified the `themesDir` property in the `config.toml`. Make sure to comment out `themesDir` in the config file if you use the theme in production. [Read more](/README.md#setup)

The addition of the `disableComments` variable in the frontmatter the comment section can be disabled on individual pages.


### 11th March 2017

- Update hightlight.js and fontawesome
- Add Gitlab and Trello icon

### 5th August 2016

**This change requires Hugo v0.16 or greater**. The Gravatar image required the manual creation
of an MD5 hash in order to generate an avatar. Now, this is done automatically. The avatar still
depends on the `gravatar` variable in the config file.
