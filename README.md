# SASS Demo Project

This is just a simple SASS demo project displaying some of the organisational capabilities that [dart-sass](https://github.com/sass/dart-sass) has to offer.

This is by no means the *ultimate* way to organise your projects, just a general idea of how I personally like to organise them.

## Structure

I organise my SASS projects with a `main.scss` file as the "entry point" of the project. This file is what ties everything together. Assuming I don't import a whole lot of external assets (e.g. fonts) I'll generally import them here.

This is also where I configure simple globals, like themes (e.g. `[data-theme=dark] {...}`) and html/body values. 

Following that, I import typography configuration/classes, layout config/classes, and finally individual components.

The `Abstracts` folder contains SASS specific values, stuff that ultimately doesn't enter into the final CSS file. This includes things like variables, mixins, and functions.

Depending on the size/scope of the project, I may sometimes divide up the `_variables.scss` file into different files.

The remaining folders are pretty self-explanatory.