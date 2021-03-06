# Contribution Guidelines

There are not many contribution guidelines but here are some helpers and how we build the Yeoman generator.

## Basic technologies to know

* [Write your own Yeoman generator](http://yeoman.io/authoring/) - This provide you some basic insights how to write a custom Yeoman generator

* [Mocha getting started](https://mochajs.org/#getting-started) - To test the Yeoman generator work properly a testing framework named Mocha is used

* [Embedded JavaScript templating](http://ejs.co) - Is the core engine used in Yeoman do deploy template files and dynamically embed custom settings in the files getting deployed.

## Places to look for help
The JavaScript a Yeoman generator uses is based on NodeJS and many things are treated differently than the JavaScript that exists in browsers.

* [Yeoman API Documentation](http://yeoman.io/generator/) - 
Beside the getting started guide there is an official documentation availabe that cover the complete Yeoman API.

* [NodeJS documentation](https://nodejs.org/dist/latest-v8.x/docs/api/) -
In general a Yeoman generator is written is JavaScript but it is based on NodeJS the developmeent patterns are slightly different. In some cases it might be handy to consult the NodeJS documentation.

## Frequently asked questions

### Why can't I use TypeScript?
TypeScript requires compilation to JavaScript. The result is in more complexity and less support from the Yeoman community. To keep it plain and simple only NodeJS JavaScript will be used. Most concepts such as classes can be used in NodeJS anyway.

### Do I need to install @microsoft/generator-sharepoint?
No - The PnP SPFx generator has a dependency on a specific version on @microsoft/generator-sharepoint. This version will be automatically installed in the generator source.

### Can I have a different versions of @microsoft/generator-sharepoint installed?
Yes you can for example have version 1.4.1 installed manually on your machine. When you run `yo @microsoft/sharepoint` this version will be used. However in case you like to run `yo @pnp/spfx` the version the community generator was built on will be used. For example version 1.6 instead.

