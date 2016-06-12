# tooltipster-scrollableTip

A [Tooltipster](http://iamceege.github.io/tooltipster/) plugin to make tooltips scrollable when they get too big. MIT license.

When the tooltip is about to overflow the viewport, this plugin does the following: put the tooltip on the side which maximizes its size, resize it so it doesn't overflow the viewport, and make it scrollable for the content to be accessible.

The tooltip will go off screen only if the origin itself goes off screen.

Installation
------------

Include the plugin file in your page AFTER the Tooltipster bundle file.

```html
<html>
    <head>
        ...
        <script type="text/javascript" src="tooltipster/dist/js/tooltipster.bundle.min.js"></script>
        <script type="text/javascript" src="tooltipster-scrollableTip/tooltipster-scrollableTip.min.js"></script>
    </head>
</html>
```

> This plugin only works in conjunction with Tooltipster's default `sideTip` plugin.

Usage
-----

Declare the `scrollableTip` plugin in the options of the tooltips you want to be scrollable, alongside `sideTip`:

```javascript
$('.tooltip').tooltipster({
    plugins: ['sideTip', 'scrollableTip']
});
```

> Pro tip: for a better style, know that the scrollbar is customizable with CSS in Chrome

Simple as that!