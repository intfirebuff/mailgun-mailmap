# Mailgun Mailmap

[![Build Status](https://travis-ci.com/intfirebuff/mailgun-mailmap.svg?branch=master)](https://travis-ci.com/intfirebuff/mailgun-mailmap)

Mail configuration for ifba.org.

This repository contains mail configuration for ifba.org. All our mail is
handled by [Mailgun](https://www.mailgun.com/). On Mailgun, most our mail goes
through mailing lists. This means that email sent to an email address for
ifba.org is then broadcast to a list of members. We also use Mailgun routes for
handling messages intended for a single recipient. This allows an email sent to
`treasurer@ifba.org` (for example) to be forwarded to a personal mailbox.

Configuration of mailing lists is done via this git repository. The
[`mailmap.toml`](https://github.com/intfirebuff/mailgun-mailmap/blob/master/mailmap.toml)
file contains a description of all mailing lists for the ifba domains. Each
mailing list has a list of members as well.

Updates to this repository should be done through pull requests. Anyone can send
a pull request!

When a pull requests is merged Travis will run and will sync the state of
`mailmap.toml` to Mailgun itself.
