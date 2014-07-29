RequireJS template for Jasmine unit tests
-----------------------------------------

This fork manipulates the script file name before it is required in the template.

In our project, the scripts are loaded from a `baseUrl` of `lib`. The `app` prefix is mapped to `..`. In order to get the scripts to load correctly in the jasmine-requirejs template, instead of requiring them as `scripts/whatever.js`, it needs to require it as `app/whatever.js`.

There didn't seem to be a way to make this work in the original project, hence this fork.