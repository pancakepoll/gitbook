---
description: Thank you for expressing your interest in contributing to PancakePoll!
---

# Contributing

![](../../.gitbook/assets/NEWBAN.jpg)

PancakePoll is an open-source project. If you want to contribute to the project, this section is here to guide you through your first steps with the PancakePoll team 🥞

Before starting any development, we highly encourage you to submit an issue on Github in order to discuss the problem and the solution with the team. If you want to reach out to the dev team directly, [contact @AntonioPancakepoll](https://t.me/AntonioPancakepoll) on Telegram.

## Setup your dev environment

1. Fork the repository and an [add upstream remote](https://docs.github.com/en/free-pro-team@latest/github/collaborating-with-issues-and-pull-requests/configuring-a-remote-for-a-fork). E.g.

```
$ git remote add upstream git@github.com:pancakepoll/pancakepoll-frontend.git
```

&#x20; 2\. Make sure you have the latest version of the default branch ( `develop` or `master` )

```
$ git checkout develop
$ git pull upstream develop
```

&#x20; 3\. Create your own branch and install dependencies

```
$ git checkout -b branch-name
$ yarn
```

&#x20; 4\. Happy coding 🎉

## Coding rules

We try to maintain as much consistency as we can between each of our repository. Your pull request has more chances to be accepted if you follow some the following rules, and write high quality code.&#x20;

**Let's get started** 💪

## Committing <a href="committing" id="committing"></a>

## Creating your pull request

Your code is ready to be submitted for review, congratulations🥳

* All pull requests **must** have a description of what the PR is trying to accomplish.
* Keep pull requests **as small as possible**. Larger pull requests should be broken up into smaller chunks with a dedicated base branch. Please tag the PR's that are merging into your base branch with the `epic` tag.
* If possible self-review your PR and **add comments** where additional clarification is needed.

{% hint style="info" %}
Create a [draft PR](https://github.blog/2019-02-14-introducing-draft-pull-requests/) as soon as possible so we can view your ongoing progress.
{% endhint %}

**Thanks for helping us making PancakePoll even more awesome** ❤
