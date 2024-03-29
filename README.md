[![Coverage Status](https://coveralls.io/repos/SockDrawer/SockBot-Emoji/badge.svg?branch=master)](https://coveralls.io/r/SockDrawer/SockBot-Emoji?branch=master)
[![Docs Status](https://readthedocs.org/projects/sockbot-emoji/badge/?version=latest)](http://sockbot-emoji.readthedocs.org/)

# SockBot Emoji

Emoji plugin for [SockBot](https://sockbot.rtfd.org/en/latest/) version 2.11.0 or later; automatically replaces Unicode emoji with Discourse emoji in a user's posts.

## Usage

No special syntax is required; simply post as normal.

## Developers

SockBot Emoji is developed by [SockDrawer](https://github.com/SockDrawer) developer [RaceProUK](https://github.com/RaceProUK).

## Installation

The preferred method of installation is via NPM; simply run this command within the SockBot installation folder:
```
npm install sockbot-emoji
```

Other methods of installation are possible e.g. cloning the git repository, but only installation via NPM is supported.

### Post Install Setup

If you installed via NPM skip this step as NPM has already installed all necessary dependencies.
Otherwise you will need to run the following command in the folder where you installed SockBot Emoji:
```
npm install
```

## Configuration

SockBot Emoji requires no special configuration; all that is needed is a single line in the SockBot configuration file.

YAML example:
```
---
core:
  username: username
  password: password
  owner: owner
plugins:
  sockbot-emoji: true
```

JSON example:
```
{
  "core": {
    "username": "username",
    "password": "password",
    "owner": "owner"
  },
  "plugins": {
    "sockbot-emoji": true
  }
}
```

Note that these examples assume an NPM-based installation; other installation methods may require the path to `Emoji.js` (without file extension) be specified explicitly.

YAML example:
```
---
core:
  username: username
  password: password
  owner: owner
plugins:
  '../path/to/Emoji': true
```

JSON example:
```
{
  "core": {
    "username": "username",
    "password": "password",
    "owner": "owner"
  },
  "plugins": {
    "../path/to/Emoji": true
  }
}
```

## Special Thanks

For creating [SockBot](https://sockbot.readthedocs.org/en/latest/) and just generally being awesome: [Accalia de Elementia](https://github.com/AccaliaDeElementia)
