---
layout: post
title: Software on my work laptop (2025 edition)
subtitle: Nothing fancy, really!
date: 2025-08-21
---

Here is a list of software installed on my work computer. Nothing fancy or super secret. Plenty of free and open source goodies below. Let me illustrate you don't need super secret tools to develop and test software that is used by thousands of people.

## Browser: Firefox (and a few other browsers)

Firefox desktop release has been my daily driver. I may use Firefox nightly for trying out beta features.

In case of <a href="https://webcompat.com/">web compatibility</a> issues, I have Chrome/Chromium to compare with.

## Password Manager: 1Password

1Password has been my trusted tool for storing my passwords and my team's shared credentials. Never, ever share password via email or any chat software.

1Password is Canadian. 🇨🇦

## iOS development: Xcode and iOS simulators

Xcode, the official iOS development tool, is available through Apple. I use the iOS command line tool, including `xcodebuild` and `xcrun`, on a daily basis and on the CI/CD systems.

Most of my end-to-end testing has been done via the iOS simulators. I also have a physical iPad just in case of bugs that cannot be shown on the simulators. (By the way, iPad is a great external monitor.)

## IDEs: VSCode

VSCode has been my favourite IDE for many languages including Python and bash. It is lightweight. It supports many languages out of the box. The default settings are good enough for most situations.

I am also a Vi user. ;-)

## AI: Github Co-pilot and ChatGPT

Github co-pilot is a useful integration to give the AI some context to my queries. In addition, multiple AI vendors such as Claude, Gemini and ChatGPT are available from the same place readily.

ChatGPT has been helping me to research on a specific question, organize the information and brainstorm on a topic. As always, the onus is on me to prompt ChatGPT with the queries providing as much information from me as possible and ask it to be critical (instead of patronizing) in the answers.

## Package management: pyenv, venv, nvm

Different projects depends on different versions of the compilers. In addition, the dependencies of different projects may conflict between each other. The ability of switching between compiler versions and a set of dependencies are useful.

For Python, `pyenv` allows me to switch between different Python versions without reinstalling Python when I switch between different projects. Each project has its own `venv`.

For node, `nvm` manages all node installations.

## Command line goodies

The theme of my command line is from [oh my zsh](https://ohmyz.sh/). I have been treaking my command line prompt for years, but have given up to leave the task to the pros.

[brew](http://brew.sh/) installs the commands that are not included in macOS.
* `xcodes`: Install iOS runtimes and simulators without Xcode.
* `gh` and `git`: Use git from the command line.
* `bitrise`: Verify `bitrise.yml` before pushing the changes to my branch.