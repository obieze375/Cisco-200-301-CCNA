# Router Configuration

A router is configured like so:

```text
enable password !Password@1!
enable secret Password@2
line console 0
password Password@2
line vty 0 15
login
password Password@1
service password-encryption
```

Another user has been asked to examine the running configuration on the same router but not make any configuration changes. The user connects to it by using Telnet.



