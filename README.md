# Brick

Brick is the CSS toolkit that powers Wealthsimple's front-end design. It's purposefully limited to common components to provide our developers with the most flexibility. It's built with SCSS and available via Bower, so it's easy to include all or part of it within your own project.

[**Read the Brick documentation**](http://brick.wealthsimple.com/) to learn more.

## Install

Use [bower](http://bower.io/) to install the latest version of Brick on a project:

```
$ bower install --save git@github.com:wealthsimple/brick.git
```

To update the package once installed:

```
$ bower update wealthsimple-brick
```

## Usage

Once installed, simply `@import` either the master SCSS file, or the individual files as you need them.

```scss
// Example: All of Brick
@import "wealthsimple-brick/scss/brick";

// Example: Individual files
@import "wealthsimple-brick/scss/variables";
@import "wealthsimple-brick/scss/mixins";
@import "wealthsimple-brick/scss/base";
```

## Fonts

Since font installation may vary based on the asset compilation framework you're using (e.g. Sprockets for Rails, Grunt for Ghost.org), Brick does not include `@font-face` definitions. You must include these yourself.

Example below. Note: for Sprockets-based compilation, you'll want to replace `url` with `font-url`.

```scss
@font-face {
  font-family: 'FuturaBT-Light';
  src: url('/fonts/2F4FAE_0_0.eot');
  src: url('/fonts/2F4FAE_0_0.eot?#iefix') format('embedded-opentype'),url('/fonts/2F4FAE_0_0.woff2') format('woff2'),url('/fonts/2F4FAE_0_0.woff') format('woff'),url('/fonts/2F4FAE_0_0.ttf') format('truetype');
}

@font-face {
  font-family: 'FuturaBT-Book';
  src: url('/fonts/2F4FAE_1_0.eot');
  src: url('/fonts/2F4FAE_1_0.eot?#iefix') format('embedded-opentype'),url('/fonts/2F4FAE_1_0.woff2') format('woff2'),url('/fonts/2F4FAE_1_0.woff') format('woff'),url('/fonts/2F4FAE_1_0.ttf') format('truetype');
}

@font-face {
  font-family: 'FuturaBT-Heavy';
  src: url('/fonts/2F4FAE_2_0.eot');
  src: url('/fonts/2F4FAE_2_0.eot?#iefix') format('embedded-opentype'),url('/fonts/2F4FAE_2_0.woff2') format('woff2'),url('/fonts/2F4FAE_2_0.woff') format('woff'),url('/fonts/2F4FAE_2_0.ttf') format('truetype');
}

@font-face {
  font-family: 'CaslonGraD';
  src: url('/fonts/2F4FAE_3_0.eot');
  src: url('/fonts/2F4FAE_3_0.eot?#iefix') format('embedded-opentype'),url('/fonts/2F4FAE_3_0.woff2') format('woff2'),url('/fonts/2F4FAE_3_0.woff') format('woff'),url('/fonts/2F4FAE_3_0.ttf') format('truetype');
}
```

## Credits

Boilerplate for this repository was heavily reused from GitHub's own CSS toolkit: https://github.com/primer/primer