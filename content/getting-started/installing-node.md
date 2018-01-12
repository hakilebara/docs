<!--
title: 02 - How to install npm & manage npm versions 
-->

#How to Install npm & Manage npm Versions

npm is written in Node.js, so you need to install Node.js in order to use npm. You can install npm via the Node.js website, or by installing a _Node Version Manager_ or NVM. This chapter explains both options.  

# Installing npm from the Node.js site

##1. Install Node.js & npm

If you're using OS X or Windows, use one of the installers from the [Node.js download page](https://nodejs.org/en/download/). Be sure to install the version labeled **LTS**. Other versions have not been tested with npm. 

![DOSPIC](/images/win-installing-node-lts.png)
	
If you're using Linux, you can also find installers by scrolling on the [Node.js download page](https://nodejs.org/en/download/), or you can check [NodeSource's binary distributions](https://github.com/nodesource/distributions) to see if there's a more recent version that works with your system.
	
After installing, run `node -v`. The version should be higher than v8.9.1

## 2. Update npm

When you install node.js, npm is automatically installed, too. However, npm gets updated more frequently than Node.js, so you'll want to make sure it's the latest version.

To test,  run `npm -v`. Compare this version with the version at the bottom of each page of doc (scroll down) to see if it's the latest version.

If the version is not the latest version, run:

`npm install npm@latest -g`

# Using a Version Manager to install Node.js and npm

Since npm and node.js products are managed by different entities, updates and maintenance can become complex. Also, the Node.js installation process installs npm in a directory that doesn't have global permissions. This can cause permissions errors when you attempt to run packages globally. 

To solve both these issues, many developers opt to use a *node version manager*, or *nvm*, to install npm. The version manager will avoid permissions errors, and will solve the complexities of updating Node.js and npm. 

In addition, developers can use an nvm to test their applications on multiple versions of npm. The nvm enables you to easily switch npm as well as node versions.This makes it easier to ensure that your applications work for most users, even if they are using other versions of npm. Use the instructions for the version manager you select to learn how to switch versions, and to learn how to keep up-to-date with the latest version of npm. 

## Apple macOS 

Click [here](https://github.com/creationix/nvm/blob/master/README.md#installation) to learn how to install nvm for MacOs.  

## Microsoft Windows 
 
To install and manage npm and Node.js on Windows, we suggest this version manager,[nvm-windows](https://github.com/coreybutler/nvm-windows).

## Linux 

Click [here] (https://github.com/creationix/nvm/blob/master/README.md#installation) to learn how to install nvm for Linux.

# Experimenting with the Next Release 

*For more advanced users*

If you want to try the next, unreleased version of npm to test packages you have created, use this command:

`npm install npm@next -g`

This may simply reinstall the current version, depending on the development cycle. 

## Learn More

To learn how to use nvm, click [here](https://github.com/creationix/nvm/blob/master/README.md#usage).


