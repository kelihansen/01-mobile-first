Lab 01: Mobile First
=======

Welcome to your first lab assignment for Bootcamp: Part Two!!

Today we'll be kicking off our blog app by applying what we learned in lecture to implement a mobile-first design using responsive web design techniques. You'll also need to spend some time getting familiar with the new Git/GitHub & Pair Programming workflow that we'll utilize throughout this course.

*Please take the time to read carefully through each of the READMEs for lab assignments as they have detailed information regarding your assignment, such as: submission instructions, resources, configuration, and user stories with feature tasks.*

## Content
1. Pairing Flow and Submission Instructions
1. Configuration
1. User Stories and Feature Tasks

---

## Pairing Flow and Submission Instructions
Read through the pairing flow and submission instructions outlined in our [submit-process repo](https://github.com/alchemy-bootcamp-two-winter-2018/submit-process).

---

## Configuration
_Your repository must include:_

- `README.md` - with information about your repo (follow the README template in our [submit-process repo](https://github.com/alchemy-bootcamp-two-winter-2018/submit-process))
- `.gitignore` - with standard NodeJS configurations
- `.eslintrc.json` - with our course standards for the linter

```
01-mobile-first/starter-code/
├── .eslintrc.json
├── .gitignore
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
│   ├── modules.css
│   ├── state.css
│   └── theme.css
└── vendor
    └── styles
        └── normalize.css
```


--

## User Stories and Feature Tasks

*As a user, I want to have an application that looks good, is easy to use, and is updated often, so that I want to come back and use it frequently.*

- Working from the provided [comp images](comp-images/), write CSS such that the browser rendering matches the images as closely as possible.
- Utilize the icon fonts located in `styles/icons.css` for navigation features as shown in the comp images.

*As a developer, I want to use standard industry practices for setting up and organizing the code that handles the styling of my application so that it is easy to edit and maintain.*

- Utilize a [`normalize.css`](https://github.com/necolas/normalize.css/blob/master/normalize.css) file, which should be placed in a `vendor/styles/` directory, to override default browser settings that affect the way documents render.
- Utilize SMACSS practices to organize CSS into separate files and appropriately order the loading of those files in the `<head>` of the HTML document. At minimum you should have a file for: base, layout, and module styles.

*As a user, I want a familiar experience of the application so that I know how to use it on my smartphone and occasionally my laptop.*

 - Initially design the application to render per the comp images on mobile devices.
 - Set up the viewport and fluid media rules so content renders per the comp images in both mobile and desktop views. Use a breakpoint of 640 pixels.
 - Add a "Hamburger" menu button that reveals the nav links when tapped on a mobile device.
- Ensure that images are responsive and do not exceed the size of the viewport.


### Stretch Goals
*As a user, I want a familiar experience when accessing the application on my tablet so that I can get the most out of the screen size.*
- Set up an intermediate media query for tablet devices (choose the maximum width at your own discretion).

*As a developer, I want to stay up to date with the latest in CSS features.*
- Instead of using clearfix to make my article images stay within the article containers, I want to use the newer CSS display property that does a similar thing. 

*As a developer I want to use SMACCS to its fullest.*
- Categorize your styles into state and theme files.