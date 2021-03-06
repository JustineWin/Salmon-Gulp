# Salmon Boilerplate (Gulp)


This boilerplate is Justine Win's custom version of Devtip's Starter Kit V2.

Salmon uses Jade (Pug) and Sass and includes clean flex layout classes, optional bootstrap & skeleton grid, and what-not.

If you're not yet into Jade, Sass, nor Gulp, try this [one](https://github.com/JustineWin/Salmon/tree/Salmon-v2).

##Grids

Choose whether you want to use bootstrap's or skeleton's grid then go to main.sass file and comment out the grid's css file you will not use

##Flex layout

This page is using flex classes. I have included helpful comments on the flex-layout.sass file. Go ahead, experiment!

##Getting started


### Requirements
This project have some requirements you need to meet in order to compile it. First of all, you need NodeJS in order to run javascript on the console, you can go to the [NodeJS](http://nodejs.rg) site and follow trough the installation process. After you get the `node` command on the console, you need to install Gulp and Bower globally with the following command.

```
node install -g gulp bower
```

Gulp is the one that will run all the compilation, watchers and others tasks. Bower will get the dependencies for the client side like jQuery. Those are the only requeriments to run this project.


### Download Zip

Download the zip file then open the project on your terminal. Type in

```
npm install && bower install
```

Wait for the dependencies to install.

type in `gulp build` then `gulp start`. You should be able to run it on your localhost:3000 

Start building!

### Clone

I do not recommend cloning yet, there seems to be an error regarding the gulpfile. Will look into this. 


## How to use
To start using it, the only thing you need to do is open the project on you code editor of choice and code. To compile and live preview all your changes you have some command that will help you. Here are the list of commands you should know.

Every command have to be executed on the root directory of the project using the gulp command like `gulp clean` or `gulp build`

* **start**: Compile and watch for changes (For development)
* **clean**: Removes all the compiled files on ./build
* **js**: Compile the JavaScript files
* **jade**: Compile the Jade templates
* **sass**: Compile the Sass styles
* **images**: Copy the newer to the build folder
* **favicon**: Copy the favicon to the build folder
* **vendors**: Copy the vendors to the build folder
* **build**: Build the project
* **watch**: Watch for any changes on the each section
* **help**: Print this message
* **browsersync**: Start the browsersync server

If you are in development, the `gulp start` command is the best choice for you. Go to the project folder in the console and execute `gulp start`, it will compile the project and start a server that will refresh every time you change something in the code. Gulp will be watching for changes and will tell you how to access the project from local and public url. Every browser that point to that url will be auto refreshed. As an extra feature for testing purpose any interaction on one browser will be reflected on any others. Try it on a phone, tablet and pc at the same time.

## Structure
The project have a very simple and flexible structure. If the default place for any file or directory needs to be moved, be sure to update to the new position on the config file.

```
├───build -> All the compiled files will be placed here (Distribuction)
│   ├───assets -> Compiled Assets
│   ├───index.html -> Compiled Jade files
│   ├───vendors -> Project dependencies
├───source -> Source files for the project
│   ├───assets -> Assets for the project
│   │   ├───img -> Images
│   │   └───js -> Scripts
│   ├───sass  -> Sass styles
│   │   └───main.sass -> Main file in where all other sass files should be included.
│   ├───vendors -> Vendors folder for all the dependencies (Managed by Bower)
│   └───views -> Templates directory for Jade files
│   │   └───index.jade
├───.bowerrc -> Define where the dependencies will be installed
├───bower.json -> Bower configuration file for manage project dependencies
├───package.json -> NodeJS configuration file for manage node dependencies
├───gulpfile.js -> Gulp Tasks
├───config.js -> Project configuration
```
All the files in the build folder will be auto-generated by the different tasks when the project compiles. Be sure to not modify any file manually in the build folder because changes will be replaced on the compile process.

## Configuration
This project have some nice configuration options to meet all you needs. To configure you need to edit the `config.js` file and change any value you need. Every aspect of this configuration is described in the file so that you know the options.

##Future Plans

Will include an image minifier soon and yeoman for fast installation.

### Inspired by

This is inspired by [Travis Neilson's](https://github.com/travisneilson)  Devkit. Visit [DevTipsStarterKit.com](http://devtipsstarterkit.com) for more info.

### Original Gulp version
DevTipster [Maikel José Rivero Dorta](https://github.com/mriverodorta) created a [gulp version](https://github.com/mriverodorta/DevTips-Starter-Kit/tree/Gulp-Starter-Kit), and a [Command Line Interface](https://github.com/mriverodorta/devtips-cli) for this project!! So cool :)
