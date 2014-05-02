---
layout: page
title: The Environment
previous: ".."
next: "../2-providers"

---

When working with Juju, what you are actually managing is a cloud environment.
This is not just the services you have running in your deployment, but also all
of the metadata that goes along with them, their machines, how they talk and
relate to each other, whether or not they're exposed to the public, and so on.
You can think of an environment as being analogous to a literal environment,
complete with different species and interactions, with overall and individual
health, and so on.

You can also think of an environment as a structural diagram of your cloud
deployment abstracted into different services and applications.  In fact, that's
precisely the way it works within Juju:

[![A sample deployment with three
services](sample-deployment.png)](sample-deployment.png)

> A sample deployment with three services in the Juju graphical user interface
> (GUI)

Each of the boxes in the above diagram represents a service.  A service is an
abstract concept that represents an application, web service, or workload
deployed to the cloud on one or more machines, whether that's on a container
such as LXC or KVM, on a virtual machine or cloud image, or on bare metal.

For now, you can see the start of our cloud-based press-release site running on
Ghost.  This shows the Ghost platform - a Node.js based blog - connected to
haproxy, which is exposed to the world, as well as the Juju GUI service, which
is currently showing this environment.  You can see that Ghost is not exposed,
however since haproxy is, and Ghost is connected to haproxy through a relation
powered by the HTTP interface (more on these later), you can still get to the
website as haproxy shows it.  Juju GUI, which is not related to anything, also
needs to be exposed in order to see this view of the environment.
