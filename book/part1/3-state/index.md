---
layout: page
title: The State Server
previous: "../2-providers"
next: "../4-bootstrapping"

---

The Juju state server\* is the heart of your deployment.  It manages everything
about your environment:

* Services and their configuration values
* Relations between services
* Units and what machines or containers they are placed on
* Machines and their constraints and tags
* Containers and their types and what machines they are on
* Status of all of the above
* Any additional annotations on various 

The state server is what is created when you type `juju bootstrap` from the
command line (thus its older name, the "bootstrap node"), and maintains all of
the state of your environment.  You can think of it as the master of the entire
operation: it knows where everything is located, its general state, how it is
set up, and so on.  It's rather like a spider in that sense, as all of the Juju
agents on all of the machines or containers talk back to it along their
connections to the state server, and the state server can talk back by deploying
a unit of a service to that machine.
