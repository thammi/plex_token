# Plex Token

## Introduction

This script assists you in generating a [Plex](https://plex.tv) authentication
token. Other tools like
[plex-sync](https://github.com/jacobwgillespie/plex-sync) can use these tokens
to access your account.

# Usage

  Usage: ./plex_token CLIENT USER [PASSWORD]

The `CLIENT` id is used to identify the token in the devices section of your
Plex account. Requesting a token for an existing client id will return the
existing token. `USER` is your Plex username and `PASSWORD` is your password. If
you omit the password on the command line you will be asked to input it
interactively, which is the recommended way to use this tool.

## Technical Notes

The token is requested using the method described
[here](https://forums.plex.tv/discussion/129922/how-to-request-a-x-plex-token-token-for-your-app/p1).
The `CLIENT` parameter is used as client identifier and product name. The
version is hardcoded to 0.0.1.

