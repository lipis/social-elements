Open Graph Elements and More
============================

> Everything you would like to include to make your website more social.

Contents
--------

- [Facebook](#facebook)
- [Favicon](#favicon)
- [GitHub buttons](#github-buttons)
- [Open Graph](#open-graph)
- [Twitter](#twitter)

Facebook
--------

### Buttons

Include this preferably before the `</body>` for any Facebook buttons.

```html
<div id="fb-root"></div>
<script>(function(d, s, id) {
  var js, fjs = d.getElementsByTagName(s)[0];
  if (d.getElementById(id)) return;
  js = d.createElement(s); js.id = id;
  js.src = "//connect.facebook.net/en_US/sdk.js#xfbml=1&version=v2.6&appId=<APP_ID>";
  fjs.parentNode.insertBefore(js, fjs);
}(document, 'script', 'facebook-jssdk'));</script>
```

#### Like Button
For more information head to [Like Button](https://developers.facebook.com/docs/plugins/like-button).

```html
<div class="fb-like" data-href="https://developers.facebook.com/docs/plugins/" data-layout="standard" data-action="like" data-show-faces="true"></div>
```

Additionally you can include `data-share="true"` if you want to shares well.

The `data-layout` can also be `box_count`, `button_account`, `button`.

#### Follow Button

For more information head to [Follow Button](https://developers.facebook.com/docs/plugins/follow-button).

```html
<div class="fb-follow" data-href="https://www.facebook.com/lipis" data-layout="standard" data-show-faces="true"></div>
```

Additionally you can include `data-width` and `data-height`.

The `data-layout` can also be `box_count`, `button_account`, `button`.

Favicon
-------

For the main favicon itself, it's best for cross-browser compatibility not to use any HTML. Just name the file favicon.ico and place it in the root of your domain.

For more information head to [favicon-cheat-sheet](https://github.com/audreyr/favicon-cheat-sheet).

GitHub buttons
--------------

For more information head to [GitHub buttons](https://ghbtns.com/).

### Star

```html
<iframe src="https://ghbtns.com/github-btn.html?user=lipis&amp;repo=social-elements&amp;type=star&amp;count=true" frameborder="0" scrolling="0" width="170px" height="20px"></iframe>

<iframe src="https://ghbtns.com/github-btn.html?user=lipis&amp;repo=social-elements&amp;type=star&amp;count=true&amp;size=large" frameborder="0" scrolling="0" width="160px" height="30px"></iframe>
```

### Watch

```html
<iframe src="https://ghbtns.com/github-btn.html?user=lipis&amp;repo=social-elements&amp;type=watch&amp;count=true&amp;v=2" frameborder="0" scrolling="0" width="170px" height="20px"></iframe>

<iframe src="https://ghbtns.com/github-btn.html?user=lipis&amp;repo=social-elements&amp;type=watch&amp;count=true&amp;size=large&amp;v=2" frameborder="0" scrolling="0" width="160px" height="30px"></iframe>
```

### Fork

```html
<iframe src="https://ghbtns.com/github-btn.html?user=lipis&amp;repo=social-elements&amp;type=fork&amp;count=true" frameborder="0" scrolling="0" width="170px" height="20px"></iframe>

<iframe src="https://ghbtns.com/github-btn.html?user=lipis&amp;repo=social-elements&amp;type=fork&amp;count=true&amp;size=large" frameborder="0" scrolling="0" width="158px" height="30px"></iframe>
```

### Follow

```html
<iframe src="https://ghbtns.com/github-btn.html?user=lipis&amp;type=follow&amp;count=true" frameborder="0" scrolling="0" width="170px" height="20px"></iframe>

<iframe src="https://ghbtns.com/github-btn.html?user=lipis&amp;type=follow&amp;count=true&amp;size=large" frameborder="0" scrolling="0" width="220px" height="30px"></iframe>
```

Open Graph
----------

For more information head to [The Open Graph protocol](http://ogp.me/).

### Basic Metadata

```html
<meta property="og:type" content="website">
<meta property="og:url" content="https://github.com/lipis/social-elements">
<meta property="og:title" content="Social Elements">
<meta property="og:description" content="Social Elements">
<meta property="og:image" content="https://lipis.github.io/social-elements/social-elements.png">
```

### Optional Metadata

- `og:audio` — A URL to an audio file to accompany this object.
- `og:determiner` — The word that appears before this object's title in a sentence. An enum of (a, an, the, "", auto). If auto is chosen, the consumer of your data should chose between "a" or "an". Default is "" (blank).
- `og:locale` — The locale these tags are marked up in. Of the format language_TERRITORY. Default is en_US.
- `og:locale:alternate` — An array of other locales this page is available in.
- `og:site_name` — If your object is part of a larger web site, the name which should be displayed for the overall site. e.g., "IMDb".
- `og:video` — A URL to a video file that complements this object.

Twitter
-------

### Buttons

For more information head to [Twitter buttons](https://about.twitter.com/resources/buttons).

Include this preferably before the `</body>` for any Twitter buttons.

```html
<script>!function(d,s,id){var js,fjs=d.getElementsByTagName(s)[0],p=/^http:/.test(d.location)?'http':'https';if(!d.getElementById(id)){js=d.createElement(s);js.id=id;js.src=p+'://platform.twitter.com/widgets.js';fjs.parentNode.insertBefore(js,fjs);}}(document, 'script', 'twitter-wjs');</script>
```
#### Share a link

```html
<a href="https://twitter.com/share" class="twitter-share-button" data-via="Lipis">Tweet</a>

<a href="https://twitter.com/share" class="twitter-share-button" data-url="https://github.com/lipis/social-elements" data-text="Everything that you need to make your website social friendly" data-via="Lipis" data-size="large" data-hashtags="opengraph">Tweet</a>
```

#### Follow

```html
<a href="https://twitter.com/Lipis" class="twitter-follow-button" data-show-count="false">Follow @Lipis</a>

<a href="https://twitter.com/Lipis" class="twitter-follow-button" data-show-count="false" data-size="large">Follow @Lipis</a>
```

#### Hashtag

```html
<a href="https://twitter.com/intent/tweet?button_hashtag=SocialElements" class="twitter-hashtag-button" data-related="Lipis">Tweet #SocialElements</a>

<a href="https://twitter.com/intent/tweet?button_hashtag=SocialElements&amp;text=Everything%20you%20would%20like%20to%20include%20to%20make%20your%20website%20more%20social" class="twitter-hashtag-button" data-related="Lipis" data-url="https://github.com/lipis/social-elements" data-size="large">Tweet #SocialElements</a>
```

#### Mention

```html
<a href="https://twitter.com/intent/tweet?screen_name=Lipis" class="twitter-mention-button" data-related="Lipis">Tweet to @Lipis</a>

<a href="https://twitter.com/intent/tweet?screen_name=Lipis&amp;text=Hello%2C%20World!" class="twitter-mention-button" data-size="large" data-related="Lipis">Tweet to @Lipis</a>
```
