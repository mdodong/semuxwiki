### General configuration

```
################################################################################
#                                                                              #
# Copyright (c) 2017 The Semux Developers                                      #
#                                                                              #
# Distributed under the MIT software license, see the accompanying file        #
# LICENSE or https://opensource.org/licenses/mit-license.php                   #
#                                                                              #
################################################################################

#================
# P2P
#================

# Declared ip address
p2p.declaredIp =

# Binding IP address and port
p2p.listenIp = 0.0.0.0
p2p.listenPort = 5161

# Seed nodes, IP addresses separated by comma
p2p.seedNodes =


#================
# Network
#================

# Max number of inbound connections
net.maxInboundConnections = 1024

# Max number of outbound connections
net.maxOutboundConnections = 128

# Max message queue size
net.maxMessageQueueSize = 4096

# Message relay redundancy
net.relayRedundancy = 16

# Channel idle timeout
net.channelIdleTimeout = 120000

#================
# API
#================

# Be sure to set up authentication first before enabling API
api.enabled = false

# Listening address and port
api.listenIp = 127.0.0.1
api.listenPort = 5171

# Basic authentication
api.username = YOUR_API_USERNAME
api.password = YOUR_API_PASSWORD
```

### IP whitelist and blacklist

Example:
```
{ 
    "rules": [
        {"type": "ACCEPT", "address": "127.0.0.1/8"},
        {"type": "ACCEPT", "address": "192.168.0.0/16"},
        {"type": "REJECT", "address": "8.8.8.8"}
    ]
}
```