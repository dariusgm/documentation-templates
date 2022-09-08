# general documentation for company example

This is just a [template](https://github.com/dariusgm/documentation-templates).

You may not need every aspect of the template, but they give you an idea what *can* be documented in your projects.

    Good documentation reflect any granularity of your project.

## Pre Installation

This section describe topics that need to be done before you can install anything. For example, how you get the hardware, credentials for login.

## Installation

Here you define the actual installation steps, reference a script or
a framework that does the installation required.

Take into account that you may need to support different operating systems.
Run this installation steps against a Dockerfile in a CI environment, to
make sure its updated and running. When commands can't be tested on CI,
use `|| true` to ignore the status code of the previous command. Use it
with caution.


## Post Installation

Some tasks can not be done in an automatic fashion.
You may need to enter user specific credentials or even generate something by yourself.
This steps should be written in this area.

Also setting up the recommended editor(s) with their settings can help
in the collaboration. This can be from code style to editor memory settings.

## Snippets

And here is some space for writing down snippets. Remember, this are
code chunks and need to be "completed" by somebody using them.
* What are you regularly running that may be forgotten as its long or complicated?
* What are pattern you are using for reading or writing files?
* What you use to do argument parsing?

[source](https://github.com/dariusgm/documentation-templates)
