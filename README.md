# Homebrew-test

Testing homebrew taps for python apps

## Why not submit PRs to Homebrew/homebrew?

This is lighter weight with less overhead to publishing new versions.
Plus the author is in full control, can experiment as needed, etc.

The only downsides are *slightly* more typing for a user to install and not being discoverable
as part of the main homebrew repo.

## Updating mapbox-cli-py

    mkvirtualenv brewit
    pip install mapboxcli
    pip install homebrew-pypi-poet
    poet -f mapboxcli > ~/work/homebrew-test/Formula/mapbox.rb

## Installation

```
brew install <user>/<repo-minus-homebrew>/mapbox
```

So if my username is `perrygeo` and my repo is `homebrew-test`, install with 

```
brew install perrygeo/test/mapbox
```
Which will automatically "tap" my repository

## Reference

[Python for Formula Authors](https://github.com/Homebrew/homebrew/blob/master/share/doc/homebrew/Python-for-Formula-Authors.md)
[How to create and maintain a tap](https://github.com/Homebrew/homebrew/blob/master/share/doc/homebrew/How-to-Create-and-Maintain-a-Tap.md)


