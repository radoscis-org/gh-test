# TO READ
https://docs.github.com/en/actions/managing-issues-and-pull-requests/using-github-actions-for-project-management
https://docs.github.com/en/actions/creating-actions/creating-a-docker-container-action

https://semver.org/
https://www.conventionalcommits.org/en/v1.0.0/
https://rednafi.github.io/digressions/python/2020/04/06/python-precommit.html

HOW TO CREATE REUSABLE TEMPLATES

# Actions for Workflows
https://github.com/actions

# Actions Marketplace
https://github.com/marketplace?type=actions

https://github.com/actions/hello-world-javascript-action

# Virtual Envs
https://docs.github.com/en/actions/using-github-hosted-runners/about-github-hosted-runners

# Software installed on runners
https://docs.github.com/en/actions/using-github-hosted-runners/about-github-hosted-runners#supported-software

# Managing workflow runs (Debugging)
https://docs.github.com/en/actions/managing-workflow-runs#enabling-debug-logging

# Workflow syntax for GitHub Actions
https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions#using-a-specific-shell

# Events that trigger workflows
https://docs.github.com/en/actions/using-workflows/events-that-trigger-workflows

# Create a repository dispatch event
https://docs.github.com/en/rest/repos/repos#create-a-repository-dispatch-event

# Filter pattern cheat sheet
https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions#filter-pattern-cheat-sheet

# Environemnt Variables
https://docs.github.com/en/actions/learn-github-actions/environment-variables

# Automatic token authentication
https://docs.github.com/en/actions/security-guides/automatic-token-authentication

# Encrypted Secrets
Secret can be only 64 KB
What if we have bigger file for eg to keep as secret ?
https://docs.github.com/en/actions/security-guides/encrypted-secrets
https://www.gnupg.org/

We use gpg
```
gpg --symmetric --cipher-algo AES256 secret-test.json
# Will ask for passphrase that should be kept as secret in GH Actions
# Now we can push file into repo
```

# Expression Contexts and Functions and Job Status Functions
https://docs.github.com/en/actions/learn-github-actions/contexts
https://docs.github.com/en/actions/learn-github-actions/expressions#functions
https://docs.github.com/en/actions/learn-github-actions/expressions#status-check-functions


# Caching workflow dependencies
https://docs.github.com/en/actions/using-workflows/caching-dependencies-to-speed-up-workflows


# Publishing dockers
https://docs.github.com/en/actions/publishing-packages/publishing-docker-images

# CUSTOM ACTIONS
## TOOLKIT for building custom acitons
https://github.com/actions/toolkit

npm i @actions/github --save
npm i @actions/core --save



### Core package description
https://github.com/actions/toolkit/tree/master/packages/core

# ACTIONS USED IN COURSE
https://github.com/actions/setup-node
https://github.com/actions/cache


# Repos and additions used


# Workflow commands for GithubActions
https://docs.github.com/en/actions/using-workflows/workflow-commands-for-github-actions

# Octokit/rest.js

Github API rest client !
It is inside github package
https://octokit.github.io/rest.js/v18/

## Semantic release tool
https://github.com/semantic-release/semantic-release

npm install --save-dev semantic-release
release.config.js

 npx semantic-release

## Semantic versioning
https://semver.org/
## Conventional commits
https://www.conventionalcommits.org/en/v1.0.0/

## Commitizen
https://github.com/commitizen/cz-cli

npm install commitizen -g
commitizen init cz-conventional-changelog --save-dev --save-exact


 "config": {
    "commitizen": {
      "path": "cz-conventional-changelog"
    }
  }

It will help us create proper commits

>When you commit with Commitizen, you'll be prompted to fill out any required commit fields at commit time. No more waiting until later for a git commit hook to run and reject your commit (though that can still be helpful). No more digging through CONTRIBUTING.md to find what the preferred format is. Get instant feedback on your commit message formatting and be prompted for required fields.

## Commit Lint
https://github.com/conventional-changelog/commitlint
https://www.freecodecamp.org/news/how-to-use-commitlint-to-write-good-commit-messages/

It will lint our commits , run hook and prevent improper commits before sending them into git

commitlint checks if your commit messages meet the [conventional commit format](https://conventionalcommits.org/)

## Simple nodejs api dockerized
https://github.com/alialaa/simple-docker-nodejs-api

## Create React App
https://create-react-app.dev/

npx create-react-app react-app --use-npm

## Deploy static website - surge
https://surge.sh/

angry-babies.surge.sh

surge list
surge token
surge whoami

## Use Prettier for Code formatting rules
https://prettier.io/

 npx prettier --write "**/*.js"
 npx prettier --check "**/*.js"

## Upload code coverage reports into service
CodeCov

## NPM CI
https://docs.npmjs.com/cli/v8/commands/npm-ci

# MARKETPLACE
## Action Versioning
https://github.com/actions/toolkit/blob/master/docs/action-versioning.md

## Icons
https://feathericons.com/