# GULP Workflow

## Instructions

1. Make sure you have these installed
	- [node.js](http://nodejs.org/)
	- [gulp](http://gulpjs.com/) 
	- [bower](https://bower.io/) 

2. Clone this repository into your local machine:

git clone https://jmoracuc@bitbucket.org/jmoracuc/intercollegiate-cms-landing-page.git newprojectname/

3. CD to the folder newprojectname

4. Run `> npm install` to install npm project dependencies

5. Run `> bower install` to install bower project dependencies

6. Run '> gulp' command to start project 

7. Fire up your browser at `http://localhost:8080`

##  Workflow

Working localhost folder is builds/development/
This is where you want to add any html/php files or images into images/

To edit CSS do so from components/sass/ 

_mixins.css // add any mixins in here
_screen.scss // all main styles in here
_typography.scss // imports google font
_variables // colors and such defined

After any change to an html/php, js or scss file the browser will auto-refresh

##  Production deployment

1. Stop gulp server if its running '> CTRL + C'

2. Run the Gulp command `>NODE_ENV=production gulp`
This will compile all files from builds/development/ into builds/production.

Processes:
a) Images minified
b) html minified
c) javascript concatenated and minified
d) css minified

Note: The command line will print the processes as they execute, keep an eye on them in case there are any errors. 