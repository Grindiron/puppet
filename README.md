# About

This private Git repository contains the necessary configuration files
for deploying a functional, "standalone" Puppet instance.

All machine instances that are intended to be running on a long-term basis or as
part of a self-taught technical investigation will have their complete deployment and
configuration specified in a declarative manner.


# "Standalone" deployment model

In order to accelerate initial operationalisation I have adopted the
"standalone" Puppet instance deployment model as outlined in the "Puppet 5
Beginner's Guide 3rd Edition" book.

This approach requires each host intending to configure itself via Puppet to
first pull the entirety of this Git repository and run the initial `bootstrap.sh`
script.
Depending on the operational complexity I encounter in the future I may transition
the deployment model to the officially recommended, albeit more complex, 
"Master & Agent" model.


# Github

The purpose of the private Github repository
(https://github.com/Grindiron/puppet) is to mirror the locally hosted Git
repository. *All* host deployments relying on Puppet driven configuration will
will pull from the read-only, anonymous accessed, locally hosted Git repository.
