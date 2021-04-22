---
title: Setup
lang: en-US
description: 'How to install Bricks WordPress starter theme'
---

# {{ $frontmatter.title }}

## Requirements

- [Git](https://git-scm.com/) to clone this repository.
- [Yarn](https://yarnpkg.com/) as the preferred tool to manage dependencies and run development scripts (you can also use plain [npm](https://nodejs.org/)).
- [Gulp-cli](https://github.com/gulpjs/gulp-cli) installed globally to run individual sub-tasks (Optional).

## Installation

- Clone Bricks from its [repository](https://github.com/stefanobartoletti/bricks) directly inside the `wp-content/themes` directory in your WordPress installation:

    ```bash
    git clone -b master https://github.com/stefanobartoletti/bricks.git
    ```
    ::: tip
    The `-b master` argument is required to set `master` as the main branch, tracking the latest released version.
    
    However, the main branch of the GitHub repository is `devel`, that instead is used for development purposes and against which Dependabot Pull Requests are made.
    :::

- Delete `.git` and `.github` directories inside the newly created `bricks` theme folder.
  
- Run `git init` to initialize a new repository from scratch (you may skip this step, i.e. if you already have a Git repository versioning your entire WordPress installation).

- Install dependencies with your package manager (the install script will also perform the initial setup):

    <code-group>

    <code-block title="Yarn" active> 
    ```bash
    yarn install
    # or simply
    yarn
    ```
    </code-block>

    <code-block title="npm"> 
    ```bash
    npm install
    ```
    </code-block>
    
    </code-group>