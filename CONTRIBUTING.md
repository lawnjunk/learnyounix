Contributing to learnyounix
=================================

### Table Of Contents
* [Code of Conduct](#code-of-conduct)  
* [Report Issues](#report-issues)  
* [Suggestions and Requests](#suggestions-and-requests)  
* [Your First Contribution](#your-first-contribution)  
* [Pull Requests](#pull-requests)
* [Style Guide](#styleguide)  

## Code of Conduct
This project adheres to the Contributor Covenant [code of conduct](CONDUCT.md). You are expected to uphold this code.  
Please report unacceptable behavior to **dwolfm@gmail.com**.

## Report Issues
#### Before you report an issue, try to debug it
* search your error on [duckduckgo](https://duckduckgo.com)  
* search your error on [stackoverflow](http://stackoverflow.com/)  

#### Where to submit your issue
If you find a spelling issue, error, bug, or any other issue with any of the current documents.  
Open a new issue in the [Waffle](http://waffle.io/slugbyte/learnyounix) and place it in the **Issues** column.  

#### How to submit a "good" issue
* Use a clear **descriptive title**
* Describe the **exact steps** which reproduce the problem
 * Don't just say what you did, but explain **how you did it**! 
* Provide **specific examples** to demonstrate the steps
 *  Include links to files or GitHub projects, copy/pasteable snippets. If you provide snippets in the issue use [markdown code blocks](https://help.github.com/articles/basic-writing-and-formatting-syntax/#quoting-code)
* Provide **screenshots**
* Provide your **Operating System** and its **version**
* Provide the **shell** you are using and its **version**
* Provide the **command(s)** you used and their **version(s)**
* Provide links to any resources you found helpful **while trying to debug your error**!
 * Provide the solution that worked for you! **:)**
 
## Suggestions and Requests
#### Before you make a request for new content
* Use Github's search in project feature to search our project for your topic
* Double check the readme titles to make sure your topic isn't covered
* Research the topic so you can point us in the right direction

#### Where to submit your Request
Open a new issue in the [Waffle](http://waffle.io/slugbyte/learnyounix) and place it in the **Suggestion** column.

#### How to make a "good" request
* Use a clear **descriptive title**
* Describe **why your request will help developers**
 * Not just that you want to know how something works 
* Provide **links to any resources** you find helpful regarding your topic

## Your First Contribution
**Not sure what to work on?** You can start by looking at the [Waffle](http://waffle.io/slugbyte/learnyounix) board for beginner issues.  
**Not sure how to contribute?** Learn to [fork a repo](https://help.github.com/articles/fork-a-repo/), then learn about [using pull requests](https://help.github.com/articles/using-pull-requests/).

## Pull Requests
 * Create an Issue on [Waffle](http://waffle.io/slugbyte/learnyounix)
 * Follow the [Styleguide](STYLEGUIDE.md)
 * [Write a good commit message](http://chris.beams.io/posts/git-commit/)
  * First line should be less than 50 characters
  * Have an empty second line and then a summary
  * In the summary answer these questions: _Why is this change necessary?_, and _How does it address the issue?_ 
  * Add a link referencing the [Waffle](http://waffle.io/slugbyte/learnyounix) issue.

## Styleguide
file names: `**filename**` -> **unicorn.md**  
file extension: `**.ext**` -> **.md**  
literal string: `'string'` -> `'**/*.js'`  
inline command: `command` ->  `grep`


command description: `$ command` -> `$ ls`  
argument description: `<argument description>` -> `$ ls <flag>`  
optional argument: `<optional argument description>` -> `$ ag ... <optional file/dir name>`  

examples
```
> ``` sh
> # description of what you are going to accomplish
> $ command <arg1> <arg2>
> ``` 
```
->
``` sh
# use grep to filter history for the occurences of the word 'curl'

$ history |grep 'curl'
```

