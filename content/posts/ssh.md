+++
title = 'Basic SSH guide'
date = 2023-12-04T20:01:33-08:00
draft = false
+++

This is how I would set up ssh in a local network

**First, this post assumes that you have ssh server installed, on whatever machine you are using.**


After installing the openssh-server package onto your device, make sure that it is activated by using:


```
sshd
```
as a root user in linux/macos or 
```
Start-service sshd
```
In an admin powershell

## Next steps

Once that is done, you can use another terminal-ready device or an ssh client to connect to the remote linux server. For example, install openssh-client to access a remote system over the network.

After that, use this command and replace the values with the ones you need.

```shell
ssh REMOTE_USERNAME@IPADDRESS
```
This works if the remote server is broadcasting on port 22, which it generally is unless something has been modified by the server admin.

After that, you can manipulate the terminal of the remote machine running ssh-server.

It really is a cool technology.
