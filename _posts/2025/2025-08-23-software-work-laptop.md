---
layout: post
title: Software on my work laptop (2025 edition)
subtitle: Nothing fancy, really!
date: 2025-08-21
---

Here's the software on my work computer. Nothing fancy or secret—just practical tools that anyone can download and run for free.  Let me illustrate how anyhelp me develop and test software used by thousands of people.

## Browser: Firefox (and a few others)

Firefox desktop is my daily driver. I use Firefox Nightly for beta features.

For [web compatibility](https://webcompat.com/) issues, I keep Chrome/Chromium and Safari around for comparison.

## Password Manager: 1Password

1Password stores my passwords and my team's shared credentials. Never share passwords via email or chat.

Plus, 1Password is Canadian. 🇨🇦

## iOS Development: Xcode and simulators

Xcode is the official iOS development tool. I use iOS command line tools like `xcodebuild` and `xcrun` daily, both locally and in CI/CD.

Most end-to-end testing happens on iOS simulators. I keep a physical iPad for bugs that don't show up in simulators. (Pro tip: iPads make great external monitors.)

## IDE: VS Code

VS Code is my go-to for Python, bash, and other languages. It's lightweight, supports many languages out of the box, and the defaults work well.

I'm also a Vi user. ;-)

## AI: GitHub Copilot and ChatGPT

GitHub Copilot gives AI context about my code. It also provides access to multiple AI vendors (Claude, Gemini, ChatGPT) in one place.

ChatGPT helps with research, organizing information, and brainstorming. I always provide detailed context and ask it to be critical rather than just agreeable.

## Package Management: pyenv, venv, nvm

Different projects need different compiler versions and dependencies that often conflict.

For Python: `pyenv` switches between Python versions, and each project gets its own `venv`.

For Node: `nvm` manages all Node installations.

## Command Line Tools

My shell theme comes from [oh my zsh](https://ohmyz.sh/). After years of tweaking prompts, I let the pros handle it.

[Homebrew](http://brew.sh/) installs tools not included in macOS:
* `xcodes`: Install iOS runtimes and simulators without Xcode
* `gh` and `git`: Command line Git tools
* `bitrise`: Verify `bitrise.yml` before pushing changes