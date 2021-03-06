# Text Heavy Webpage Template

> Built for presenting content that is information dense, easily updatable, and optimized for legibility, this template has a sticky horizontal top nav on mobile, feature callouts, cards and a site map footer with a deep-linked table of contents.

[http://www.getmdl.io/templates/index.html](http://www.getmdl.io/templates/index.html)


To use this template execute from your command line:
```
dnu restore
```
The `postrestore` scripts in `project.json` will install client side dependencies to the project. The MDL will be installed locally via Bower package manager and then its core main files will be moved to project web site root.

```
dnu build
```

**NOTE** On Mac OS X I'd advice to build and run project using `CoreCLR` to avoid `Mono` problems with files watcher. You could do this way under `RC1`:

```
dnvm use -r coreclr 1.0.0-rc1-final
dnu restore
dnu build --framework dnxcore50
```
This 'prebuild' scripts in the `project.json` will clean existing and create new minified version of client-side JavaScript and CSS files

To run project:
```
dnx web
```

Thanks!
