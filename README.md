# device-minecraft
Provides a Minecraft Java server appliance

The appliance provides one or more installations of the Minecraft Java edition server.

This appliance does the following:

- All parameters passed to the device commands are syntax checked and canonicalised, with bash completion.
- Installs one or more Minecraft servers with the given name and port.
- Autostarts on server restart.

## before

- Deploy the device-minecraft package.

```
[root@server ~]# dnf install device-minecraft
```

## add

To add the appliance, run this.

```
[root@server ~]# device services app add name=myserver
```

## remove

To remove the appliance, run this.

```
[root@server ~]# device services app remove myserver
```

## show

To show the current configuration, run this.

```
[root@server ~]# device services app minecraft show 
Flags: disabled (X)
      NAME  PORT     PROTOCOL  
  myserver        prefer-ipv6  
```

