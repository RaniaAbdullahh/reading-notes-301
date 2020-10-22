## Heroku
Heroku is a platform as a service (PaaS) that enables developers to build, run, and operate applications entirely in the cloud. Developers use Heroku to build, deliver, monitor, deploy, manage, and scale modern apps.
## Defining an application

Heroku lets you deploy, run and manage applications written in Ruby, Node.js, Java, Python, Clojure, Scala, Go and PHP.

An application is a collection of source code written in one of these languages, perhaps a framework, and some dependency description that instructs a build system as to which additional dependencies are needed in order to build and run the application.
> Dependency mechanisms vary across languages: in Ruby you use a Gemfile, in Python a requirements.txt, in Node.js a package.json, in Java a pom.xml and so on.

The source code for your application, together with the dependency file, should provide enough information for the Heroku platform to build your application, to produce something that can be executed.
## Knowing what to execute
You don’t need to make many changes to an application in order to run it on Heroku. One requirement is informing the platform as to which parts of your application are runnable.

If you’re using some established framework, Heroku can figure it out. For example, in Ruby on Rails, it’s ``typically rails`` server, in Django it’s python ``<app>/manage.py runserver`` and in Node.js it’s the ``main`` field in package.json.
## Deploying applications
Git is a powerful, distributed version control system that many developers use to manage and version source code. The Heroku platform uses Git as the primary means for deploying applications (there are other ways to transport your source code to Heroku, including via an API).

When you create an application on Heroku, it associates a new Git remote, typically named ``heroku``, with the local Git repository for your application.

As a result, deploying code is just the familiar ``git push``, but to the ``heroku`` remote instead:

``$git push heroku master``
-----------------
