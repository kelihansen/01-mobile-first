Lab 01: Mobile First
=======

Welcome to your first lab assignment for Code 301!!

Today we'll be kicking off our blog app by applying what we learned in lecture to implement a mobile-first design using responsive web design techniques. You'll also need to spend some time getting familiar with the new Git/GitHub & Pair Programming workflow that we'll utilize throughout this course.

*Please take the time to read carefully through each of the READMEs for lab assignments as they have detailed information regarding your assignment, such as: submission instructions, resources, configuration, user stories with feature tasks, and documentation.*

## Content
1. Pairing Flow
1. Resources
1. Configuration
1. User Stories and Feature Tasks
1. Documentation

---

## Pairing Flow

Here is the recommended workflow:

**Set up your repo**

1. Driver: fork the class org's lab repository if you haven't done so already.
    * Your **forked repo** on GitHub is your `origin` repo.
    * Be sure to add your navigator as a collaborator (go to `Settings` -> `Collaborators & teams`) so they can push directly to it.
1. Clone **your fork** to your local development environment. Follow this directory <span id="directory">structure</span>:

	```
	~/acl
	  301/
	    lab-assignments/
	      01-mobile-first/ # this is the cloned repository for today's work
	```

1. Immediately `git checkout -b <feature-name>` (ex: `git checkout -b responsive-design`).

**Write code together!**

1. In VS Code use the "Find in Project" feature (`CTRL/CMD + SHIFT + F`) to locate all the `TODO:`, `REVIEW:`, and `COMMENT:` items.
1. Before writing code, read-through the existing code and discuss the `REVIEW` items with your partner.
1. Start `live-server` in your terminal to render the code in the browser. 
    * Note that `live-server` will automatically update the browser when code is changed and saved.
1. Work through one or two `TODO` or `COMMENT` items before switching roles (or one hour, whichever arrives first), testing your code as you go.
1. Do an A-C-P cycle:
    1. `git add` the changes that you've made.
    1. `git commit -m "some meaningful message"` where some meaningful message is a message that **thoroughly** explains your commit.
    1. `git push origin <branch-name>` to push your branch to your forked repo on GitHub.

**Switch roles**

The navigator (who will become the new driver):

  - Clone your pair's fork from GitHub.
    - See the above <a href="#directory">directory structure</a> for what you should have on your file system.
  - Fetch the branch you were just working on (`git fetch origin <feature-name>`)
  - Checkout that branch (`git checkout <feature-name>`).
  - Open the code in your editor and resume editing the code.
  - Add, commit, push as you have done before.


---

## Resources  
<!-- a list of links if any are necessary for the assignment-->
- [Video: Mobile Testing Tip for Your Phone](https://www.youtube.com/watch?v=2t4E_tc8TKM)

---

## Configuration
_Your repository must include:_

- `README.md` - with documentation regarding your lab and its current state of development. Check the "documentation" section below for more details on how that should look **AT MINIMUM**
- `.gitignore` - with standard NodeJS configurations
- `.eslintrc.json` - with Code 301 course standards for the linter

```
01-mobile-first/starter-code/
├── .eslintrc.json
├── .gitignore
├── LICENSE
├── README.md
├── index.html
├── styles
│   ├── base.css
│   ├── fonts
│   │   ├── icomoon.eot
│   │   ├── icomoon.svg
│   │   ├── icomoon.ttf
│   │   └── icomoon.woff
│   ├── icons.css
│   ├── layout.css
│   └── modules.css
└── vendor
    └── styles
        └── normalize.css
```


--

## User Stories and Feature Tasks

*As a user, I want to have an application that looks good, is easy to use, and is updated often, so that I want to come back and use it frequently.*

- Working from the provided [comp images](comp-images/), write CSS such that the browser rendering matches the images as closely as possible.
- Utilize the icon fonts located in `styles/icons.css` for navigation features as shown in the comp images.

*As a developer, I want to use standard industry practices for setting up and organizing the code that handles the styling of my application so that my code is easy to edit and maintain.*

- Utilize a [`normalize.css`](https://github.com/necolas/normalize.css/blob/master/normalize.css) file, which should be placed in a `vendor/styles/` directory, to override default browser settings that affect the way documents render.
- Utilize SMACSS practices to organize CSS into separate files and appropriately order the loading of those files in the `<head>` of the HTML document.

*As a user, I want a familiar experience of the application so that I know how to use it on my smartphone and occasionally my laptop.*

 - Initially design the application to render per the comp images on mobile devices.
 - Set up the viewport and fluid media rules so content renders per the comp images in both mobile and desktop views. Use a breakpoint of 640 pixels.
 - Add a "Hamburger" menu button that reveals the nav links when tapped on a mobile device.
- Ensure that images are responsive and do not exceed the size of the viewport.


### Stretch Goal
<!-- Include any additional stretch goals for this assignment, which can vary depending on the class and their overall preparedness for additional work. -->
*As a user, I want a familiar experience when accessing the application on my tablet so that I can get the most out of the screen size.*
- Set up an intermediate media query for tablet devices (choose the maximum width at your own discretion).

---

## Documentation  
_Your README.md must include:_

```md
# Project Name

**Author**: Your Name Goes Here
**Version**: 1.0.0 (increment the patch/fix version number up if you make more commits past your first submission)

## Overview
<!-- Provide a high level overview of what this application is and why you are building it, beyond the fact that it's an assignment for a Code Fellows 301 class. (i.e. What's your problem domain?) -->

## Getting Started
<!-- What are the steps that a user must take in order to build this app on their own machine and get it running? -->

## Architecture
<!-- Provide a detailed description of the application design. What technologies (languages, libraries, etc) you're using, and any other relevant design information. -->

## Change Log
<!-- Use this are to document the iterative changes made to your application as each feature is successfully implemented. Use time stamps. Here's an examples:

01-01-2001 4:59pm - Application now has a fully-functional express server, with GET and POST routes for the book resource.

## Credits and Collaborations
<!-- Give credit (and a link) to other people or resources that helped you build this application. -->
-->
```
