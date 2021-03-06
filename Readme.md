# attr-plugin

  [Brick](https://github.com/bredele/brick) plugin to bind a node attribute with a [store](https://github.com/bredele/store) attribute

## Installation

with [component](http://github.com/component/component):

    $ component install bredele/attr-brick

with [nodejs](http://nodejs.org):

    $ component install attr-brick

## Usage

First, add the plugin to your view (see [brick](https://github.com/bredele/brick) to know more about views):

```js
view.add('data-attr', require('attr-brick'));
```

## Basic

```html
<a data-attr="href, github"></a>
```

The plugin will look if it finds the property `github` and listen for changes.

```js
view.set('github', 'http://github.com/bredele');
```

will display:

```html
<a href="http://github.com/bredele"></a>
```
see [live example](https://github.com/bredele/attr-brick/tree/master/example)

## Alternative

[brick](https://github.com/bredele/brick) allows variable substitutions

```html
<a href="{{ github }}"></a>
```

## License

  MIT
