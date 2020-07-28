# Command Line Basics

![This is the Lab Topology used in this page.](../../.gitbook/assets/image%20%283%29.png)

## Using Cisco CLI Help

```text
Router1>
```

When pressing Enter key in the commandline the `Router1>` prompt appears.

### EXEC mode

The `>` symbol at the end indicates you are in user EXEC mode.

{% hint style="info" %}
EXEC mode is a read-only mode where you can not configure or alter the router settings. However, you can view system information and operations.
{% endhint %}

### \(?\) HELP command

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



