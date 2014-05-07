---
layout: page
title: Introduction
previous: ".."
next: "../part1"

---

Dev-ops is one of those hard problems.

(why)

Being one of those hard problems, there are countless solutions out there.  One
of these is Juju.

Juju began its life as a Python implementation, named Ensemble early on, and has
since shifted to the Go programming language, and grown into one of the largest
Go projects at the time of writing.  The goal of Juju is to distill the dev-ops
knowledge of hundreds of engineers into best-practice solutions known as charms.
Available to the user are, at time of writing, more than one hundred thirty
charms ready to use and deploy to many different cloud providers, from AWS and
HP Cloud, to your own personal OpenStack or MAAS installation within your
datacenter, down to even Linux containers running on your development laptop.

These charms have been written and contributed to by experts in dev-ops and
those particular software solutions.  The knowledge held by these developers has
been encapsulated in their charms, ensuring that the deployments of, for
example, MySQL, Ceph, or Redis will be solid and repeatable.

Many like to compare Juju to Chef, Puppet, or Ansible.  However, it would be
more accurate to say that Juju is one layer higher than those solutions.  In
fact, There are both Puppet and PuppetMaster charms, and Juju plays well with
Chef and Ansible; all of your existing Chef cookbooks and Ansible playbooks can
be used in conjunction with your own charmed or bundled project.  All of the
accumulated knowledge of your team within those areas of expertise need not go
to waste: you can use Juju alongside your own technologies with ease.

This book is intended to be both a story and a guide.  Juju has been a solid
project for more than two years now, and as such, it has a accrued a solid base
of reference documentation.  However, reference documentation does not
necessarily tell the story of one's interaction with Juju.  It is exactly what
it says on the tin: reference.

While working on the Ghost charm, what we found lacking was a comprehensive,
start-to-finish guide to both Juju as a dev-ops solution, as well as the
charming process.  It is our hope that this book will be that guide and will
help others to get up and running with their own environments and charms in the
future.

Just as Juju and its charms are open source and accepting of contributions, this
guide is open as well.  Hosted on GitHub, anyone can submit patches, errata, bug
reports, suggestions, or updates as the world of Juju and its ecosystem change
over time.  Be sure to check it out, and help contribute if you can at <a
href="http://github.com/exploring-juju">GitHub.com/exploring-juju</a>.
