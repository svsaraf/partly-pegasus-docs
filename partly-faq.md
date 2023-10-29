Partly Developer FAQ
====

## How do we make changes to the Partly codebase?

```ssh
   cd ~
   cd Projects
   sub partly_neo
   <make whatever changes you want>
   git add .
   git commit -m 'updated partly codebase'
   git push origin master
```

## How do we make changes to the Partly DOCS codebase?

* Make a change or add a new markdown file
* Add the file to index.rst

## How do I run the docs site?

```ssh
   source venv/bin/activate
   make html
   sphinx-autobuild . _build/html
```