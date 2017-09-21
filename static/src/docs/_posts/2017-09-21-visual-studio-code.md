---
layout: page
title: "Visual Studio Code"
category: use-kryptonite-with
date: 2017-09-21 15:52:45
---

# Using Kryptonite with Visual Studio Code
Both `ssh` logins and `git` PGP code signatures work out-of-the-box with Visual Studio Code.

## Disable `git` autofetch
By default, Visual Studio Code will periodically pull any git repository you have open. This creates many unnecessary Kryptonite authentication requests, and we recommend disabling this feature by adding the following to your Visual Studio Code `settings.json`:

```json
{
    "git.autofetch": false
}
```