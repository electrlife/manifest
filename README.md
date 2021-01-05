# How to create repos from manifest file

## Install repo command line
Many distros include repo, so you might be able to install from there.

# Debian/Ubuntu.
$ sudo apt-get install repo

# Gentoo.
$ sudo emerge dev-vcs/repo

You can install it manually as well as it's a single script.

$ mkdir -p ~/.bin
$ PATH="${HOME}/.bin:${PATH}"
$ curl https://storage.googleapis.com/git-repo-downloads/repo > ~/.bin/repo
$ chmod a+rx ~/.bin/repo

Or you can download it manually from code_snappiets

## Create cpp_platform repos
repo init -u https://github.com/electrlife/manifest.git -b main -m cpp_platform.xml --repo-url=https://github.com/GerritCodeReview/git-repo.git --repo-rev=main
