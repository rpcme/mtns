# mtns

A set of almost-tools that help me track changes for the meta-aws project.

mtns would mean "maintainer tracking and notification system" if we were in 70s IBM, or phonetically mean "emptyness" if living in some emo-goth echochamber.  Really, it's four characters put together that doesn't clash with anything else and it's relatively easy to remember.


## Prerequisites

1. A relatively modern GNU/Linux based system
2. git

## Basic, almost unreadable steps to almost-success

1. Clone this repo
2. modify `repos.conf` to meet your configuration needs.
3. run `reposync` to initialize the repos under `~/.mtns/repos`. You can setup a daily cron job to keep them up to date.
4. run `repotodo` to get a report of tags applied to repos in the last 7 days.  You can change the number of days by running the following with changing dayspan signified by x `repotodo x`
5. run `repodepend` to identify submodules and their aligned tags. This should help with configuring PREFERRED_VERSION_x properly.

