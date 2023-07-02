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
# Index.html loads first
Web apps need a starting point. Index.html is usually the first page to load. Let us open the file and find out what it contains. You will find it under the src folder.

<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>GettingStarted</title>
  <base href="/">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link rel="icon" type="image/x-icon" href="favicon.ico">
</head>
<body>
  <app-root></app-root>
</body>
</html>

