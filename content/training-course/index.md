---
title: Test engineering course
date: 2018-02-13T13:42:49-05:00
---

I have tried to use as few tools and helpers as possible to demonstrate a UI testing framework using only selenium-webdriver and chromedriver. And coding will be in JavaScript, though what follows can be done in other programming languages. The only either requirement is having Node and Git installed.

The assumption is you have set up accounts on Github - you can use you GitHub credentials to login to both Travis-CI and Netlify when the time comes.

While it will be important to understand running commands from a Terminal, for this training guide, using the web services will be sufficient.

## GitHub
GitHub is a code hosting platform for version control and collaboration. It lets you and others work together on projects from anywhere.

### Create a repo on github

Github is a service where you can keep your code, and make it available to others. After setting up your account, click the "+" symbol in the top-right of the menu bar.
￼
### Fill in repo form
The defaults are ok, but remember to select to add README to add repo info.

### Webpage
Create first HTML page
After creating repo, click "Create New File" and enter filename `index.html`.

Now we can start the coding!
```
<!DOCTYPE html>
<html>
  <head>
    <title>A simple website</title>
  </head>

  <body>
    <h1>Example use of [h1] element tag</h1>
    <p>Example use of [p] element tag</p>
    <p>A basic form to test search DuckDuckGo</p>
    <form action="https://duckduckgo.com/">
      <input type="text" name="q" class="searchform" />
      <button id="searchButton" type="submit">Search</button>
    </form>
    <h3>Example use of [h3] element tag</h3>
    <a href="https://duckduckgo.com">A test link</a>
    <h4>Example image</h4>
    <img src="test.png" alt="example image" />
  </body>
</html>
```
Scroll down to see lines of code highlighted, alongside explanations.
```
<!DOCTYPE html>
<html>
  <head>
    <title>A simple website</title>
  </head>

  <body>
    <h1>Example use of [h1] element tag</h1>
    <p>Example use of [p] element tag</p>
    <p>A basic form to test search DuckDuckGo</p>
    <form action="https://duckduckgo.com/">
      <input type="text" name="q" class="searchform" />
      <button id="searchButton" type="submit">Search</button>
    </form>
    <h3>Example use of [h3] element tag</h3>
    <a href="https://duckduckgo.com">A test link</a>
    <h4>Example image</h4>
    <img src="test.png" alt="example image" />
  </body>
</html>
```
DOCTYPE tells the web browser about what version of HTML the page is written in (in this case HTML5)
```
<!DOCTYPE html>
<html>
  <head>
    <title>A simple website</title>
  </head>

  <body>
    <h1>Example use of [h1] element tag</h1>
    <p>Example use of [p] element tag</p>
    <p>A basic form to test search DuckDuckGo</p>
    <form action="https://duckduckgo.com/">
      <input type="text" name="q" class="searchform" />
      <button id="searchButton" type="submit">Search</button>
    </form>
    <h3>Example use of [h3] element tag</h3>
    <a href="https://duckduckgo.com">A test link</a>
    <h4>Example image</h4>
    <img src="test.png" alt="example image" />
  </body>
</html>
```
The html element tag is called the root element because it contains all the elements in the document
```
<!DOCTYPE html>
<html>
  <head>
    <title>A simple website</title>
  </head>

  <body>
    <h1>Example use of [h1] element tag</h1>
    <p>Example use of [p] element tag</p>
    <p>A basic form to test search DuckDuckGo</p>
    <form action="https://duckduckgo.com/">
      <input type="text" name="q" class="searchform" />
      <button id="searchButton" type="submit">Search</button>
    </form>
    <h3>Example use of [h3] element tag</h3>
    <a href="https://duckduckgo.com">A test link</a>
    <h4>Example image</h4>
    <img src="test.png" alt="example image" />
  </body>
</html>
```
The head element tag contains descriptive information about the document itself, such as its title
```
<!DOCTYPE html>
<html>
  <head>
    <title>A simple website</title>
  </head>

  <body>
    <h1>Example use of [h1] element tag</h1>
    <p>Example use of [p] element tag</p>
    <p>A basic form to test search DuckDuckGo</p>
    <form action="https://duckduckgo.com/">
      <input type="text" name="q" class="searchform" />
      <button id="searchButton" type="submit">Search</button>
    </form>
    <h3>Example use of [h3] element tag</h3>
    <a href="https://duckduckgo.com">A test link</a>
    <h4>Example image</h4>
    <img src="test.png" alt="example image" />
  </body>
</html>
```
The body element tag contains everything that we want to show up in the browser window.
```
<!DOCTYPE html>
<html>
  <head>
    <title>A simple website</title>
  </head>

  <body>
    <h1>Example use of [h1] element tag</h1>
    <p>Example use of [p] element tag</p>
    <p>A basic form to test search DuckDuckGo</p>
    <form action="https://duckduckgo.com/">
      <input type="text" name="q" class="searchform" />
      <button id="searchButton" type="submit">Search</button>
    </form>
    <h3>Example use of [h3] element tag</h3>
    <a href="https://duckduckgo.com">A test link</a>
    <h4>Example image</h4>
    <img src="test.png" alt="example image" />
  </body>
</html>
```
Simple form example
```
<!DOCTYPE html>
<html>
  <head>
    <title>A simple website</title>
  </head>

  <body>
    <h1>Example use of [h1] element tag</h1>
    <p>Example use of [p] element tag</p>
    <p>A basic form to test search DuckDuckGo</p>
    <form action="https://duckduckgo.com/">
      <input type="text" name="q" class="searchform" />
      <button id="searchButton" type="submit">Search</button>
    </form>
    <h3>Example use of [h3] element tag</h3>
    <a href="https://duckduckgo.com">A test link</a>
    <h4>Example image</h4>
    <img src="test.png" alt="example image" />
  </body>
</html>
```
A text field definition for our search
```
<!DOCTYPE html>
<html>
  <head>
    <title>A simple website</title>
  </head>

  <body>
    <h1>Example use of [h1] element tag</h1>
    <p>Example use of [p] element tag</p>
    <p>A basic form to test search DuckDuckGo</p>
    <form action="https://duckduckgo.com/">
      <input type="text" name="q" class="searchform" />
      <button id="searchButton" type="submit">Search</button>
    </form>
    <h3>Example use of [h3] element tag</h3>
    <a href="https://duckduckgo.com">A test link</a>
    <h4>Example image</h4>
    <img src="test.png" alt="example image" />
  </body>
</html>
```
Add a button element with label text, to submit the form.
```
<!DOCTYPE html>
<html>
  <head>
    <title>A simple website</title>
  </head>

  <body>
    <h1>Example use of [h1] element tag</h1>
    <p>Example use of [p] element tag</p>
    <p>A basic form to test search DuckDuckGo</p>
    <form action="https://duckduckgo.com/">
      <input type="text" name="q" class="searchform" />
      <button id="searchButton" type="submit">Search</button>
    </form>
    <h3>Example use of [h3] element tag</h3>
    <a href="https://duckduckgo.com">A test link</a>
    <h4>Example image</h4>
    <img src="test.png" alt="example image" />
  </body>
</html>
```
A basic text hyperlink.
```
<!DOCTYPE html>
<html>
  <head>
    <title>A simple website</title>
  </head>

  <body>
    <h1>Example use of [h1] element tag</h1>
    <p>Example use of [p] element tag</p>
    <p>A basic form to test search DuckDuckGo</p>
    <form action="https://duckduckgo.com/">
      <input type="text" name="q" class="searchform" />
      <button id="searchButton" type="submit">Search</button>
    </form>
    <h3>Example use of [h3] element tag</h3>
    <a href="https://duckduckgo.com">A test link</a>
    <h4>Example image</h4>
    <img src="test.png" alt="example image" />
  </body>
</html>
```
Insert an image, "src" value is the path to image file.
```
<!DOCTYPE html>
<html>
  <head>
    <title>A simple website</title>
  </head>

  <body>
    <h1>Example use of [h1] element tag</h1>
    <p>Example use of [p] element tag</p>
    <p>A basic form to test search DuckDuckGo</p>
    <form action="https://duckduckgo.com/">
      <input type="text" name="q" class="searchform" />
      <button id="searchButton" type="submit">Search</button>
    </form>
    <h3>Example use of [h3] element tag</h3>
    <a href="https://duckduckgo.com">A test link</a>
    <h4>Example image</h4>
    <img src="test.png" alt="example image" />
  </body>
</html>
```
The closing tag for "body".
```
<!DOCTYPE html>
<html>
  <head>
    <title>A simple website</title>
  </head>

  <body>
    <h1>Example use of [h1] element tag</h1>
    <p>Example use of [p] element tag</p>
    <p>A basic form to test search DuckDuckGo</p>
    <form action="https://duckduckgo.com/">
      <input type="text" name="q" class="searchform" />
      <button id="searchButton" type="submit">Search</button>
    </form>
    <h3>Example use of [h3] element tag</h3>
    <a href="https://duckduckgo.com">A test link</a>
    <h4>Example image</h4>
    <img src="test.png" alt="example image" />
  </body>
</html>
```
The closing tag for "html"

### Start your website

The Node library provides a useful method of serving webpages.

Run the code, then your webpage will be ready for testing.

```
$ npm install -g http-server
$ cd /path/to/your/repo
$ http-server
Starting up http-server, serving ./
Available on:
  http://192.168.0.5:8080
  http://127.0.0.1:8080
Hit CTRL-C to stop the server
```

## Testing

Now we have a basic web page to test on!

### What to test?

On software development projects, testing work is driven by what the client has asked for.

This is a continual process that never stops, and it's important the tests reflect this.

However this not not mean testers do not manually test - on the contrary, due to the nature of UI test automation, work is constantly validated.

In further training I will go into the other sides of test automation (such as load and security testing) in future training guides.

But also it's important to remember to think creatively, and develop other useful tests (this is where developers can help you out, and will be more than happy to!).

What many testers forget, is that most developers welcome dialogue with testers, as they know how helpful they can be.

### Set up the testing framework
```
{
  "name": "javascript-chromedriver-test",
  "description": "JavaScript and Chromedriver test",
  "version": "1.0.0",
  "author": "jaffamonkey <paullittlebury@gmail.com>",
  "license": "MIT",
  "dependencies": {
    "chromedriver": "^2.46.0",
    "selenium-webdriver": "^3.5.0"
  },
  "scripts": {
    "test": "node ./test.js"
  }
}
```
For convenience to install packages, it is better to create a file `package.json` in the root of your repo, like shown here, then run npm install.
```
$ npm install
```
### To install/setup

Create a new file in `tests` folder called `test.js`. When this code is run, it first fires up Chromes browser, then excecutes the actions in the script.
```
var webdriver = require('selenium-webdriver'),
  By = webdriver.By,
  until = webdriver.until;
var errorMessage = 'Could not locate the correct ';

// This is creating an object that is the browser
const browser = new webdriver
  .Builder()
  .usingServer()
  .withCapabilities({
    'browserName': 'chrome',
    'chromeOptions': {
      args: ['headless', 'disable-gpu']
    }
  }).build();

 browser.get('http://localhost:8080')
  .then(_ =>
    // Fill in search field and hit RETURN key
    browser.findElement(By.name('q')).sendKeys('TrumpKlon', Key.RETURN))
    .then(_ => browser.wait(until.titleIs('TrumpKlon at DuckDuckGo'), 1000))
    .then(_ => browser.wait(until.elementLocated(By.partialLinkText('TrumpKlon')), 1000))
    .then(_ => browser.quit());
}
```
Although the purpose of tests varies, the context is similar:
	1.	I do something
	2.	Something happens
So test steps are (simplified) an action followed by consequence(s) - the consequence is how we verify is a test has passed or failed.
Now lets look at the lines of code in more detail ...
```
var webdriver = require('selenium-webdriver'),
  By = webdriver.By,
  until = webdriver.until;
var errorMessage = 'Could not locate the correct ';

// This is creating an object that is the browser
const browser = new webdriver
  .Builder()
  .usingServer()
  .withCapabilities({
    'browserName': 'chrome',
    'chromeOptions': {
      args: ['headless', 'disable-gpu']
    }
  }).build();

 browser.get('http://localhost:8080')
  .then(_ =>
    // Fill in search field and hit RETURN key
    browser.findElement(By.name('q')).sendKeys('TrumpKlon', Key.RETURN))
    .then(_ => browser.wait(until.titleIs('TrumpKlon at DuckDuckGo'), 1000))
    .then(_ => browser.wait(until.elementLocated(By.partialLinkText('TrumpKlon')), 1000))
    .then(_ => browser.quit());
}
The easiest way to look at this, is it's creating an object that's webdriver. Chrome will run the automated tests without UI (good for speed). headless means no browser will be visible on screen. disable-gpu means disable graphics acceleration for Chrome.
var webdriver = require('selenium-webdriver'),
  By = webdriver.By,
  until = webdriver.until;
var errorMessage = 'Could not locate the correct ';

// This is creating an object that is the browser
const browser = new webdriver
  .Builder()
  .usingServer()
  .withCapabilities({
    'browserName': 'chrome',
    'chromeOptions': {
      args: ['headless', 'disable-gpu']
    }
  }).build();

browser.get('https://localhost:8080')
  .then(_ =>
    // Fill in search field and hit RETURN key
    browser.findElement(By.name('q')).sendKeys('TrumpKlon', Key.RETURN))
    .then(_ => browser.wait(until.titleIs('TrumpKlon at DuckDuckGo'), 1000))
    .then(_ => browser.wait(until.elementLocated(By.partialLinkText('TrumpKlon')), 1000))
    .then(_ => browser.quit());
}
This is creating an object that is the browser.
var webdriver = require('selenium-webdriver'),
  By = webdriver.By,
  until = webdriver.until;
var errorMessage = 'Could not locate the correct ';

// This is creating an object that is the browser
const browser = new webdriver
  .Builder()
  .usingServer()
  .withCapabilities({
    'browserName': 'chrome',
    'chromeOptions': {
      args: ['headless', 'disable-gpu']
    }
  }).build();

 browser.get('http://localhost:8080')
  .then(_ =>
    // Fill in search field and hit RETURN key
    browser.findElement(By.name('q')).sendKeys('TrumpKlon', Key.RETURN))
    .then(_ => browser.wait(until.titleIs('TrumpKlon at DuckDuckGo'), 1000))
    .then(_ => browser.wait(until.elementLocated(By.partialLinkText('TrumpKlon')), 1000))
    .then(_ => browser.quit());
}
This is the script, the first line opens up the url, the next lines locate an element and perform an action.
var webdriver = require('selenium-webdriver'),
  By = webdriver.By,
  until = webdriver.until;
var errorMessage = 'Could not locate the correct ';

// This is creating an object that is the browser
const browser = new webdriver
  .Builder()
  .usingServer()
  .withCapabilities({
    'browserName': 'chrome',
    'chromeOptions': {
      args: ['headless', 'disable-gpu']
    }
  }).build();

 browser.get('http://localhost:8080')
  .then(_ =>
    // Fill in search field and hit RETURN key
    browser.findElement(By.name('q')).sendKeys('TrumpKlon', Key.RETURN))
    .then(_ => browser.wait(until.titleIs('TrumpKlon at DuckDuckGo'), 1000))
    .then(_ => browser.wait(until.elementLocated(By.partialLinkText('TrumpKlon')), 1000))
    .then(_ => browser.quit());
}
```
Close browser session.

### Run the tests

```
$ cd /path/to/your/test
$ node test.js
```

## Branching

At this point we have been working on the default master branch, but in order to make sure we have a stable pipeline it is better to do work and test on a separate branch.
So now create a branch called travis-ci, which will be used by Travis CI
* Go to your new repository
* Click the drop down at the top of the file list that says branch: master.
* Type a branch name, readme-edits, into the new branch text box.
* Select the blue Create branch box or hit “Enter” on your keyboard.

## Travis Build Server

Go to TravisCI

A build server (also called a continuous integration server (CI server)), is a centralized, stable and reliable environment for building software.

Developers on projects use the build server all the time, as it's the place that their code is built and tested.

Now we have the code, we need the run the tests each time the code changes, to make sure our changes don't break it.

The tests we currently start manually, but using a build server service, like Travis, these can be run automatically every time you change your code.

Basically all we have to do, is take the exact steps you did in the previous section, and put them into the simple build configuration file format.

￼
### The Travis file

Create a new file in your repo folder named `.travis.yml`

#### Add the code
```
sudo: required // Some installation actions require administrator-level access
dist: trusty // Builds a mininal machine to runs tests on

addons:
  chrome: stable // installs latest stable Chrome

language: node_js // define primary platform language

node_js:
  - '11' // define primary platform language version

branches:
  only:
  - travis-ci // Specifies that only the 'travis-ci' branch will be used

before_script:

  // install selenium-webdriver to use browser from DOM level
  - npm install selenium-webdriver

  // install chromedriver, the browser interaction service for Chrome
  - npm install chromedriver

  // Run the browser interaction service in background
  - ./node_modules/.bin/chromedriver &

script:
  - node test.js // run the tests
```
We need to write small configuration file, so that when Travis pulls the code from your GitHub repo, it knows what to do.

The file is very simple for us, so create new file in your repo called .travis.yml

After these steps are all in your code, and committed, a build process will automatically start on TravisCI

### After build
After build has completed. it will either Pass for Fail

￼
### Activate Travis build for your repo

Go to your dashboard and search for your repo
Then move switch on right so it turns green - your repo will now run through and build and test every time you change your code on GitHub.
￼
### Activate Travis build badge to your README

Add the following code to your README, and it will display the lastest Travis status for your code:

```
[![Build Status]
(https://travis-ci.org/github-userid/repo-name.svg?branch=master)]
(https://travis-ci.org/github-userid/repo-name)
```
## Deployment

Now we know out build works on the build server, it's time to deploy to Netlify, using our master, so now we need to do a Pull Request from the travis-ci branch, which when merged will trigger a deploy to Netlify (we are now going to set that up).

Strictly this would not be a deployment to live website (which I am doing here for simplicity), it would be a deployment to a test website so we can check things visually before manually deploying to live website.

## Netlify

Now log into https://app.netlify.com (you can use your GitHub account to do this)
 
* Create new GitHub repo connection
* Click the "New site from Git" button
* then click "GutHub" button (which will create connection between netlify and GitHub)

￼
## Create new deployment

Type in your repo name into search, then click on the repo link

￼
## Deploy The Site

Leave defaults, click "Deploy site" and you will see similar output to below:
￼
```
Deploy history
1:32:38 AM: Waiting to build. Currently running 1 concurrent builds on your account
1:32:38 AM: Build ready to start
1:32:40 AM: build-image version: 324ec043422499a87b63cac1f1dabeefe6dca19d
1:32:40 AM: build-image tag: v3.0.2
1:32:40 AM: buildbot version: ef2e26260c41679f4cdeaebbf93370345c9fecf7
1:32:40 AM: Fetching cached dependencies
1:32:40 AM: Failed to fetch cache, continuing with build
1:32:40 AM: Starting to prepare the repo for build
1:32:41 AM: No cached dependencies found. Cloning fresh repo
1:32:41 AM: git clone https://github.com/jaffamonkey/new-repo-name
1:32:41 AM: Preparing Git Reference refs/heads/master
1:32:42 AM: No build command found, continuing to publishing
1:32:42 AM: Starting to deploy site from '/'
1:32:42 AM: Creating deploy tree
1:32:42 AM: 2 new files to upload
1:32:42 AM: 0 new functions to upload
1:32:42 AM: Starting post processing
1:32:42 AM: Post processing done
1:32:43 AM: Site is live
```

You can now access the website, on the generated netlify url.

## Workshop files
After completing this course, you should have the following files in the root of your repo folder:

* index.html
* test.js
* package.json
* .travis.yml
￼
￼ 
