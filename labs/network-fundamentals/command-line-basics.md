# Command Line Basics

![This is the Lab Topology used in this page.](../../.gitbook/assets/image%20%283%29.png)

## Command Modes & using CLI Help

```text
Router1>
```

When pressing Enter key in the commandline the `Router1>` prompt appears.

### EXEC mode

The `>` symbol at the end indicates you are in user EXEC mode.

{% hint style="info" %}
EXEC mode is a read-only mode where you can not configure or alter the router settings. However, you can view system information and operations.
{% endhint %}

### HELP \(?\) command

By typing the question mark \(?\) key on the command-line you will show the commands that are available to you.

```text
Router1>?
access-enable            Create a temporary Access-List entry
access-profile           Apply user-profile to interface
connect                  Open a terminal connection
disable                  Turn off privileged commands
disconnect               Disconnect an existing network connection
enable                   Turn on privileged commands
exit                     Exit from the EXEC
help                     Description of the interactive help system
lock                     Lock the terminal
login                    Log in as a particular user
logout                   Exit from the EXEC
mrinfo                   Request neighbor and version information from a multicast router
mstat                    Show statistics after multiple multicast traceroutes
mtrace                   Trace reverse multicast path from destination to source
name-connection          Name and existing network connection
pad                      Open a X.29 PAD connection
ping                     Send echo messages
ppp                      Start IETF Point-to-Point Protocol (PPP)
resume                   Resume an active network connection
rlogin                   Open an rlogin connection
show                     Show running system information
slip                     Start a Serial-line IP (SLIP)
systat                   Display information about terminal lines
telnet                   Open a telnet connection
terminal                 Set terminal line parameters
```

### HELP \(\*?\) command filter

You can display commands that start with specific letters by issuing typing them in front of the question mark.

`c?` will show all commands that start with c. In EXEC mode this would be the result:

```text
Router1>c?
connect
```

`l?` would give this result:

```text
Router1>l?
lock    login    logout
```

### Priviledged EXEC mode

The `#` symbol indicates you have entered the privileged EXEC mode.

```text
Router1>enable
Router1#
```

## Abbreviations & Autocomplete

The CLI doesn't care if you don't type the full command as long as it isn't ambiguous \(i.e. matches multiple commands\).

### Typing the first few letters of a command

Try this, type `sh` into the commandline like so:

```text
Router1#sh
```

Now, press TAB

```text
Router1#show
```

The CLI have auto completed `sh` into `show` for you!

### Using abbreviated commands with help \(?\)

Now that you've learnt `sh` is short for `show` that's all fine. But the `show` command in itself doesn't do anything! 

```text
Router1#show
%Incomplete command.
```

It's a verb that is used together with other terms to form the full commands.

Try this, type `show?` into the commandline like so:

```text
Router1#show?
access-lists             List access lists
archive                  Archive functions
arp                      ARP table
auto                     Show Automation Template
cdp                      CDP information
class-map                Show QoS Class-Map
clns                     CLNS network information
clock                    Display the system clock
compress                 Show compression statistics
configuration            Contents of Non-Volatile memory
controllers              Interface controller status
crypto                   Encryption module
debugging                State of each debugging option
dhcp                     Dynamic Host Configuration Protocol status
dialer                   Dialer parameters and statistics
dmvpn                    Display DMVPN session related information
eigrp                    EIGRP show commands
event                    Embedded event related commands
flash:                   display information about flash: file system
flow                     Flow information
frame-relay              Frame-Relay information
glbp                     GLBP information
history                  Display the session command history
```





