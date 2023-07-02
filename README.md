# MyNotes
# What is a Bootstrapping
Bootstrapping is the process of initializing or loading our Angular application.
Angular takes the following steps to load our first view.

1. Loads *Index.html*
2. Loads *Angular & Third-party libraries & Application*
3. Executes application entry point (*main.ts*)
4. Load & execute Root Module (*app.module.ts*)
5. Executes the Root Component (*app.component.ts*)
6. Displayes the template (*app.component.html*)