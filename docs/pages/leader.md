# Leader

<p class="uk-text-lead">Create dot leaders for pricing menus or tables of contents.</p>

A leader, also known as a dot leader or a tab leader, is a repeating pattern used to visually connect content across horizontal spaces. They are most commonly used for restaurant menus, between the meals and prices, and for tables of contents, between titles and page numbers.

***

## Usage

To apply this component, add the `uk-leader` attribute to the left element. A line of characters, by default dots, will then fill the remaining space between the item and its adjacent element.

```html
<div uk-leader></div>
```

```example
<div class="uk-grid-small" uk-grid>
    <div class="uk-width-expand" uk-leader>Lorem ipsum dolor sit amet</div>
    <div>$20.90</div>
</div>
```

***

## Fill character

To change the dot to any custom character, just add the `fill: STRING` option to the attribute.

```html
<div uk-leader="fill: _"></div>
```

```example
<div class="uk-grid-small" uk-grid>
    <div class="uk-width-expand" uk-leader="fill: _">Lorem ipsum dolor sit amet</div>
    <div>$20.90</div>
</div>
```

***

## Responsive

It's possible to disable the leader for different device widths by applying the `media` option to the attribute and adding the appropriate viewport width. Add a number in pixel, for example `media: 640`, or a breakpoint, for example `media: @m`. The leader will be shown from the specified viewport width and upwards, but not below.

```html
<div uk-leader="media: @m"></div>
```

***

## Component options

The table below lists the available settings of the `uk-leader` attribute. [Learn more](javascript.md#component-configuration)

| Option  | Value  | Default     | Description                                                                                             |
|:--------|:-------|:------------|:--------------------------------------------------------------------------------------------------------|
| `fill`  | String | `undefined` | Optional fill character.                                                                                |
| `media` | Integer, String | `false`     | Condition for the space filling - a width as integer (e.g. 640) or a breakpoint (e.g. @s, @m, @l, @xl) or any valid media query (e.g. (min-width: 900px)). |

TODO Primary option

***

## JavaScript

Learn more about [JavaScript components](javascript.md#programmatic-use).

### Initialization

```js

```
