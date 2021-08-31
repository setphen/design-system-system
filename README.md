# Design System System

This is a lightweight boilerplate static site for documenting design systems and
component libraries.

[Demo](https://setphen.github.io/design-system-system/)

## Starting local development

1. Install [Hugo]

1. Run `hugo serve` in the root of this project

1. visit `http://localhost:1313/design-system-system`

## How it works

Design System System is a [Hugo](https://gohugo.io) project which aims to give
you just enough tooling to start documenting your design system, style guide, or
component library. This project includes as little JavaScript as possible, and
less than 200 lines of CSS, meaning that it can be easily extended and
configured to your liking.

Pages are written using markdown, and component previews are possible by
including `.rendered` and `.markup` files within the page bundle, for example:

```
content/component/button
├── button.react.markup
├── button.html.markup
├── button.rendered
└── index.md
```

Each variant of a component consists of the following:

1. __A 'rendered' file__, which is an entire HTML document that contains the
   component and will be displayed inside an iframe. This includes the markup,
   CSS, javascript, and any other resources required by the component.

1. __One or more 'markup' files__, which describe the code of the component as
   it would be used in a project. The language of the markup is included in the
   filename, for instance: `component.erb.markup` or `component.react.markup`.
