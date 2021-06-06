# `hbplugin-noloadbalancer`

A plugin to attempt to remove the need of a separate load balancer and cluster
process.

Currently experimental, as while it would be relatively easy to just allow
clients to connect directly to a worker process instead of going through
a load balancer, it would lose the functionality of plugins that use the
load balancer.

This plugin attempts to resolve that.

The plugin hooks into the `loadbalancer.beforecreate` and `loadbalancer.beforejoin`
events, and uses a fake worker node with the same socket as the load balancer.
Then, when a player creates a game, it instead creates it directly on the fake worker
node. Every other packet is sent directly into the worker node as a fake duplicated
client.