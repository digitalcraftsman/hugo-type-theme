### Type

A free and open-source ~~Jekyll~~ Hugo theme. Great for blogs and easy to customize. This theme is a port of the original [Type theme](https://github.com/rohanchandra/type-theme) made by [Rohan Chandra](https://github.com/rohanchandra). Noteworthy features of this Hugo theme are the integration of a comment-system powered by Disqus, Google Analytics and localization (l10n) support.

![](https://raw.githubusercontent.com/digitalcraftsman/hugo-type-theme/dev/images/screenshot.png)


## Get the theme

I assume you've Git installed. Inside the folder of your Hugo site run

    $ cd themes
    $ git clone https://github.com/digitalcraftsman/hugo-type-theme.git

You should see a folder called `hugo-type-theme` inside the `themes` directory that we created a few moments ago. For more information read the official [setup guide](https://gohugo.io/overview/installing/) of Hugo.


## Setup

Next, navigate to the `exampleSite` folder at `themes/hugo-type-theme/exampleSite/`.  In order to get your site running, you need to copy `config.toml` and all the content of all relevant subfolders such as `data/l10n.toml` into the root folders.

To turn the `exampleSite` folder in a standalone demo site the `themesDir` property has been set to `../..`. This way you can preview this theme by running `hugo server` inside `exampleSite` folder.

**Due to the customized `themesDir` path Hugo will fail to find themes if you copied the `config.toml` into the root directory of a regular Hugo website.** Make sure you comment out the `themesDir` property if you use the theme in production.


## The config file

Now, let us take a look into the `config.toml`. Feel free to play around with the settings.

### Comments

The optional comment system is powered by Disqus. Enter your shortname to enable the comment section under your posts.

    disqusShortname = ""

With the `disableComments` frontmatter parameter you can disable the comment section for each page individually.

### Google Analytics

The same applies to the activation of Google Analytics. Enable it by entering the tracking code for your website.

	googleAnalytics = ""


## Menu links

You can define menu entries as you like by linking a post or any other site. First, let us link a post that you've written. We can do this in the frontmatter of the post's content file by setting `menu` to `nav`. That's it.

    +++
    menu = "nav"
    +++


## Localization (l10n)

You don't blog in English and you want to translate the theme into your native locale? No problem. Take a look in the `data` folder and you'll find a file `l10n.toml` that we've copied at the beginning. It contains all strings related to the theme. Just replace the original strings with your own.


## Linking thumbnails

After creating a new post you can define a thumbnail by entering the relative path to the image in the frontmatter of the post:

    +++
    featureimage = "img/sample_feature_img.png"
    +++

This way you can store them either next to the content file or in the `static` folder.

## About page

If you want to tell your audience who you are create a new file called `about.md` under `content`. For an example look at `exampleSite/content/about.md` inside the theme folder.


## Nearly finished

In order to see your site in action, run Hugo's built-in local server.

    $ hugo server

Now enter [`localhost:1313`](http://localhost:1313) in the address bar of your browser.


## Contributing

Have you found a bug or got an idea for a new feature? Feel free to use the [issue tracker](//github.com/digitalcraftsman/hugo-type-theme/issues) to let me know. Or make directly a [pull request](//github.com/digitalcraftsman/hugo-type-theme/pulls).

Please create a separate branch for each pull request


## License

This theme is released under the MIT license. For more information read the [license](https://github.com/digitalcraftsman/hugo-type-theme/blob/master/LICENSE.md).


## Acknowledgements

Thanks to

- [Rohan Chandra](https://github.com/rohanchandra) for creating the original theme
- [Steve Francia](https:////github.com/spf13) for creating Hugo and the awesome community around the project.
- [Andy Grunwald](https://github.com/andygrunwald) for contributing numerous improvements
