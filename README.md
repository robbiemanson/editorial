# Editorial
A barebones editorial starting point.

### Install
Prerequisite: [Node.js][1]

1: Clone repo to a new project folder on your machine
```
git clone --depth 1 --origin source git@github.com:robbiemanson/editorial.git new-project-folder
```

2: Install NPM modules
```
npm install
```

3: Drag project folder into Codekit, or use whatever other CLI you want to
compile Sass assets. It's expected that you'll add your own solution for
handling assets later, be that Asset Pipeline, Grunt, Gulp, etc.

4: If using Codekit, visit [http://yourmachinename.local:5757/][2],
or whatever the URL of the locally running server is.

There's also a barebones example article format: article.html

### About
Editorial is intended to be a skeletal starting point for editorial projects;
anything centered around articles, posts, etc.

It's underpinned by [FreeAgent's CSS Utilities][3], but also uses [The Grid][4] from
the Foundation framework.

Normally we wouldn't want to target bare HTML elements with CSS because doing so
causes inheritance issues; we want to abstract markup away from specific
references to content, and use a component-based approach instead. But this
project is slightly different: it allows bare elements to be targeted when inside
a specific `Editorial` container.

This means that once you've added a publishing mechanism of your choice (e.g. a
  static site generator) you'll be able to write posts/articles as Markdown
  files and benefit from some basic styling — without having add lots of
  classes to elements. If you want more advanced styling, you can simply add the
  necessary component classes.

[1]: http://nodejs.org/download/
[2]: http://<yourmachinename>.local:5757/
[3]: https://github.com/fac/fa-css-utilities
[4]: http://foundation.zurb.com/grid.html
