# Domain Profiling

Many exploits require the profiling of an Active Directory. Once we have access to a system within a domain we can use various command to perform information gathering.

```msdos
PS C:> ipconfig /all

Windows IP Configuration

   Host Name . . . . . . . . . . . . : WIN10-DEV
   Primary Dns Suffix  . . . . . . . : snowcapcyber.local
   Node Type . . . . . . . . . . . . : Hybrid
   IP Routing Enabled. . . . . . . . : No
   WINS Proxy Enabled. . . . . . . . : No
   DNS Suffix Search List. . . . . . : snowcapcyber.local
                                       localdomain
```

We can make make use of the $net$ command to identify the domain information asscoaited with a target workstation. 

```msdos
PS C:> net config workstation
Computer name                        \\WIN10-DEV
Full Computer name                   WIN10-DEV.snowcapcyber.local
User name                            Andrew Blyth

Workstation active on
        NetBT_Tcpip_{FBBE6C05-C5CD-48F6-A739-2375485F5268} (000C294A5DC3)

Software version                     Windows 10 Pro

Workstation domain                   SNOWCAPCYBER
Workstation Domain DNS Name          snowcapcyber.local
Logon domain                         WIN10-DEV

COM Open Timeout (sec)               0
COM Send Count (byte)                16
COM Send Timeout (msec)              250
The command completed successfully.

PS C:\>
```

## Contact Details
For further information and questions please contact Dr Andrew Blyth, PhD. <ajcblyth@snowcapcyber.com>.
