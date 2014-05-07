---
layout: page
title: Part 2 - Working With Charms
previous: "../part1"
next: "1-basics"

---

We've done a good job of setting up a scalable blog to help communicate with our
customers now.  We've got Ghost up and running behind haproxy and talking to
MySQL, and we can see how everything is set up with the Juju GUI deployed to our
state server.  Now that we have that, though, it's time to look at how it all
works.  What goes into a charm?  How is it built?  And now that we have our
environment all set up, how can we make sure that this process is easily
repeated?  Let's dive into the Ghost charm itself, and take a look at bundles.

Contents
--------

* [Charm Basics](/1-basics)
* [Configuration](/2-config)
* [Hooks](/3-hooks)
    * [Install](/3-hooks/1-install)
    * [Start and Stop](/3-hooks/2-start-stop)
    * [Config Changed](/3-hooks/3-config-changed)
    * [Relations](/3-hooks/4-relations)
    * [Hook Tools](/3-hooks/5-tools)
* [Interfaces](/4-interfaces)
* [Bundles](/5-bundles)
