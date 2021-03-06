# Video

<p class="uk-text-lead">Start playing videos as they are shown or enter the viewport.</p>

The Video component offers two advanced functionalities for videos. First, it allows to pause a video whenever it's hidden with CSS and resume once it becomes visible again. In addition the video can also pause when it's not in the vieport and start playing when entering the viewport again.

Second, it allows to mute YouTube and Vimeo videos which is often needed if they are used as a background of a section.

For example the [Slideshow](slideshow.md#videos), [Lightbox](lightbox.md#content-sources) and [Cover](cover.md#video) components inherit and make use of both functionalities.

***

## Usage

To apply this component, add the `uk-video` attribute to a `<video>` element. The video will be paused whenever it's hidden with CSS and resume once it becomes visible again.

```html
<video uk-video></div>
```

```example
<button class="uk-button uk-button-default uk-margin" type="button" uk-toggle="target: +">Toggle HTML5 Video</button>

<video controls playsinline uk-video>
    <source src="//www.quirksmode.org/html5/videos/big_buck_bunny.mp4" type="video/mp4">
    <source src="//www.quirksmode.org/html5/videos/big_buck_bunny.ogv" type="video/ogg">
</video>
```

***

## Autoplay inview

To play a video when it enters the viewport and pause it again when it leaves the viewport, just add the `uk-video="autoplay: inview"` attribute to a `<video>` element.

```html
<video uk-video="autoplay: inview"></div>
```

```example
<video loop muted playsinline uk-video="autoplay: inview">
    <source src="//www.quirksmode.org/html5/videos/big_buck_bunny.mp4" type="video/mp4">
    <source src="//www.quirksmode.org/html5/videos/big_buck_bunny.ogv" type="video/ogg">
</video>
```

***

## Automute YouTube or Vimeo

To mute YouTube or Vimeo videos by default, add the `uk-video="automute: true"` attribute to the `<iframe>` element.

```html
<iframe src="" width="" height="" frameborder="0" uk-video="automute: true"></iframe>
```

```example
<button class="uk-button uk-button-default uk-margin-bottom" type="button" uk-toggle="target: +">Toggle Youtube Video</button>

<iframe src="//www.youtube.com/embed/YE7VzlLtp-4?autoplay=0&amp;showinfo=0&amp;rel=0&amp;modestbranding=1&amp;playsinline=1" width="560" height="315" frameborder="0" allowfullscreen uk-responsive uk-video="automute: true"></iframe>
```

***

### Component options

The table below lists the available settings of the `uk-video` attribute. [Learn more](javascript.md#component-configuration)

| Option     | Value           | Default | Description                      |
|:-----------|:----------------|:--------|:---------------------------------|
| `autoplay` | Boolean, String | `true`  | The video automatically plays/pauses as it's visible/hidden on the page. A value of `inview` play/pause the video as it enters/leaves the viewport. |
| `automute` | Boolean         | `false` | Automatically mute YouTube or Vimeo videos.    |

`autoplay` is the _Primary_ option and its key may be omitted, if it's the only option in the attribute value.

***

## JavaScript

Learn more about [JavaScript components](javascript.md#programmatic-use).

### Initialization

```js

```
