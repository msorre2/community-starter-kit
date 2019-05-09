# welcome bot: A Probot App
Probot
![Probot logo](https://probot.github.io/assets/logo.png)

A framework for building GitHub Apps to automate and improve your workflow.

## What it does

* Probot is a framework for building GitHub Apps in Node.js, written in TypeScript. 
* GitHub Apps can listen to webhook events sent by a repository or organization. 
* Probot uses its internal event emitter to perform actions based on those events.

## Getting started

1. [Install the bot](https://github.com/apps/welcome) on the intended repositories. The plugin requires the following **Permissions and Events**:

- Pull requests: Read & Write
- Issues: Read & Write

2. Create a .github/config.yml file to check for content of the comments:

```
# Configuration for welcome - https://github.com/behaviorbot/welcome

# Configuration for new-issue-welcome - https://github.com/behaviorbot/new-issue-welcome

# Comment to be posted to on first time issues
newIssueWelcomeComment: >
  Thanks for opening your first issue here! Be sure to follow the issue template!

# Configuration for new-pr-welcome - https://github.com/behaviorbot/new-pr-welcome

# Comment to be posted to on PRs from first time contributors in your repository
newPRWelcomeComment: >
  Thanks for opening this pull request! Please check out our contributing guidelines.

# Configuration for first-pr-merge - https://github.com/behaviorbot/first-pr-merge

# Comment to be posted to on pull requests merged by a first time user
firstPRMergeComment: >
  Congrats on merging your first pull request! We here at behaviorbot are proud of you!

# It is recommended to include as many gifs and emojis as possible!
```

You can opt out of having the bot comment on first time pull requests, pull request merges, or new issues by not filling in a value for each app's respective field.

For some inspiration about what kind of content to include in your .github/config files, check out [Electron's Configuration](https://github.com/electron/electron/blob/master/.github/config.yml).

## Need help?

If you need help using this app, we encourage you to:

- Check out the [Getting Started Guide](docs/getting-started.md) in the docs folder of this repository
- If you can't find the answer there, open an issue in this repository and add the label `question`

## Project maintainers

This project is maintained by Monalisa Octocat and friends. Use of this project under the [MIT License](LICENSE.md).
