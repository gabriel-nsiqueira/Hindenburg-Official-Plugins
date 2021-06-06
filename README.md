# Hindenburg-Official-Plugins
A mono-repo of officially maintained plugins for the [Hindenburg](https://github.com/SkeldJS/Hindenburg) Among Us server.

Currently contains 3 plugins,
* [`hbplugin-customgamecode`](https://github.com/SkeldJS/Hindenburg-Official-Plugins/tree/master/packages/hbplugin-customgamecode) -
A plugin to allow clients to select their own game code for their rooms.
* [`hbplugin-noloadbalancer`](https://github.com/SkeldJS/Hindenburg-Official-Plugins/tree/master/packages/hbplugin-noloadbalancer) -
A plugin attempting to remove the need for separate load balancer and cluster
processes, while keeping full compatibility with other plugins that may use the
load balancer.
* [`hbplugin-requirehostmods`](https://github.com/SkeldJS/Hindenburg-Official-Plugins/tree/master/packages/hbplugin-requirehostmods) -
A plugin to require clients joining a room to have the same mods as the host of
the room, ensuring that all clients process packets the same and as a soft measure
to prevent cheating.