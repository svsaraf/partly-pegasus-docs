Partly Developer FAQ
====

## How do we make changes to the Partly codebase?

```ssh
   cd ~/Projects/partly_neo

   git branch # ensure you're on branch master
   git pull origin master # ensure you're up to date with remote

   git checkout -b 'add_feature_x' #create new branch, after this make some modifications
   git add .
   git commit -m 'changes made' #add new feature
   git push origin add_feature_x
   git pr create --web #add and submit the PR, merge to master

   git checkout master # go back to master
   git pull origin master # pull changes
```

## How do we make changes to the Partly DOCS codebase?

* Make a change or add a new markdown file
* Add the file to index.rst
* git and branches are kind of unnecessary, just do the simple thing. 

```ssh
   git add .
   git commit -m 'changes made'
   git push origin main
```

## How do I run the docs site?

```ssh
   source venv/bin/activate
   make html
   sphinx-autobuild . _build/html
```

## How do I run django shell?

```ssh 
   make shell
```

## How do I add a new app?
```ssh 
mkdir ./apps/foo
python manage.py startapp foo apps/foo
rm apps/foo/apps.py
# update settings.py to add apps.foo in installed apps
# update urls.py to pull in foo views.
```

## How do I install a new python dependency
1. Add the dependency in requirements.in
```ssh 
    make requirements
```

## How to connect Postico 2 to postgres locally?
The way to connect Postico 2 to Postgres locally is first I added the ports line in Docker Compose YAML, and then I used the things in Docker Compose YAML to connect to Postgres.

partly-neo as the database
postgres as the username
postgres as the password
localhost 5432 as the host and port.

## How do I inspect Alpine variables from the console?

First select what you need:
```javscript
   
   const divElement = document.querySelector('.flex.h-screen');
   
```

Then use Alpine to pull in the data element

```javscript
   
   x = Alpine.$data(divElement)
   
```

x dot will show you all the variables and functions of the Alpine variable. 