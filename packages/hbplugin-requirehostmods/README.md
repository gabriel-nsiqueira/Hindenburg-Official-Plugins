# `hbplugin-requirehostmods`

A plugin to require clients joining a room to have the exact same mods and mod versions as the host of the room.

This plugins has 2 main goals:
- As a soft preventative measure for cheaters. It's not particularly effective for
this, however, as cheaters could easily modify Reactor to prevent their mod from
being networked.
- To ensure compatibility between all clients. It is, however, good at this for
non-malicious clients. Ensuring that all mods match up means that mods that
implement new protocol features work fine for all players.

It uses Hindenburg's built-in Reactor support so the plugin itself is small.