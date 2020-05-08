# Getting Started with Angular

## Useful Angular CLI Commands

<img src="https://malcoded.com/static/68c150aaaee9e8056f44fb81a08799ad/6bc95/angular-cli-cheat-sheet.webp">

## Bootstrapping an Angular App

Everything start with our main.ts file. This is signified in our `angular.json` file as the "main" property.

## Angular Modules

Angular uses modules to bundle up sections of the application. Each module consists of the following properties:

- declarations : Used to signify which components, derivatives, and pipes are available to this module.
- imports : Used to import other modules and expose all their exports to components of this module.
- providers : States the services that are available
- exports : What is exposed when importing this module

## Accessing Static Assets

The Angular CLI should have created a `assets` directory already. If not create it under your `src` directory. Our `assets` can actually be anywhere as long as it's referenced in our `angular.json` file under the "assets" property.