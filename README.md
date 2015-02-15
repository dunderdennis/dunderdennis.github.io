# JS Boilerplate

This is a boilerplate to be used for JS-assignments in the course. 

## Install
Make sure you have the following installed on your system:
* Virtual Box [https://www.virtualbox.org/](https://www.virtualbox.org/)
* Vagrant [https://www.vagrantup.com/](https://www.vagrantup.com/)

Clone this repro to the location you want to have the project. 

Start the virtual machine using:
`vagrant up`

SSH into the machine using:
`vagrant ssh`

Change directory to:
`cd /vagrant`

Install all dependencies (incl. Bower dependencies):
`npm install`

## Running tasks
You find all prepered tasks in package.json under "scripts".

The most relevant are:
* `npm run build` Builds the system into the "dist"-folder
* `npm run watch` Watches for changes and do browserify tasks.