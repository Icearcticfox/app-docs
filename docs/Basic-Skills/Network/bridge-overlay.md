https://stackoverflow.com/questions/40974299/what-is-the-difference-between-bridge-network-and-overlay-network


Bridge networks connect two networks while creating a single aggregate network from multiple communication networks or network segments, hence the name bridge.

Image showing bridge network https://i.stack.imgur.com/2vkli.png

In the above image Station A and Station B are connected by a bridge. Thus by using the bridge we aggregated both network in a single unit (on a high level). Bridge can even be used to create connection between networks on same host. This is generally required if the host is running multiple VM's or containers.

Overlay networks are usually used to create a virtual network between two separate hosts. Virtual, since the network is build over an existing network.

image showing overlay network https://i.stack.imgur.com/Mg0Ho.png

In the above image host A and host B are connected over an external network and an overlay network is built over that network. For example initially internet was built as an overlay over telephone lines, but now many telephone networks (using VoIP) are an overlay over internet.