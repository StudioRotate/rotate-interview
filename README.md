# Rotate° interview

This repo is to be used for Rotate°'s interview day. 

Instructions for setup and running the project can be found below.

Before you start ensure you read the recommended git process for committing and submitting your work.

All required assets (fonts, images, svgs) are included and the associated design files can be found [here](https://www.dropbox.com/s/c39ly5ac3r4g74y/rotate_interview_v1.sketch?dl=0)


## Setup

``` bash
# install dependencies
$ npm install
```

## Development

``` bash
# serve with hot reload at localhost:3000
$ npm run dev

# build for production and launch server
$ npm run build
$ npm start

# generate static project
$ npm run generate
```

## Git

At Rotate° we use Git Flow as our version control process which you may or may not be familiar with. This involves the creation and usage of  `master`, `develop` and `feature` branches. Today we're just going to use `master` and `feature` branches alongside Pull Requests to manage the submission of you work for review.

- Create your feature branch off the master branch.

    ``` bash
    git checkout -b feature/<your-name>
    ```

- As you work commit your changes to your feature branch with meaningful commit names

- When finished, push your work to the remote origin on github

    ``` bash
    git push orgin feature/<your-name>
    ```

- Finally submit a Pull Request on github by navigating to <https://github.com/StudioRotate/rotate-interview>


> This project is structured using the Nuxt.js framework. For a detailed explanation on how things work, checkout [Nuxt.js docs](https://nuxtjs.org).
