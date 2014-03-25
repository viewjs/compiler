# Compiler

A cross-platform (Browser + Node) view compiler.


## Intro

Viewjs is quite simple and consistent. It works with data attributes for most of it's bindings with the ability to use interpolation `{{}}` where need be; such as within attributes, etc...

### data-text

```html
<title data-text="title"></title>
```

This binds `title` to the title tag. This assumes that the `title` variable/property is accessible from within that scope.


## Scoping

By default, each view creates a new scope. Scoping allows you to isolate some properties from others. For example, when you have sub-views, iterations, etc...

You can manually create a new scope through `data-scope`.

```html
<div data-scope="someScope"></div>
```

Iterations, also create a new scope per loop:

```html
<span data-each="user in users" data-text="user"></span>
```


# License

MIT
