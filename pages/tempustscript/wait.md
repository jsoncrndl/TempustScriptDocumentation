---
title: The Wait Command
tags: [wait, pause, delay, seconds]
keywords:
summary: "Pause the script for some number of seconds"
sidebar: tempustscript_sidebar
permalink: wait.html
folder: tempustscript
toc: false
---

# The "wait" Command
The wait command pauses script execution for the given amount of seconds.

**Usage**

    wait time_in_seconds

## Example

    say["Counter"] "Got a minute?"
    wait 60
    say "Thank you for your time."