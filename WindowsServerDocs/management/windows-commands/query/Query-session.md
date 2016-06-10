---
title: Query session
ms.custom: na
ms.prod: windows-server-2012
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: abc0ace8-0b74-4b6e-a937-a78bb4b61a1f
---
# Query session
Displays information about sessions on a Remote Desktop Session Host \(RD Session Host\) server.

The list includes information not only about active sessions but also about other sessions that the server runs.

For examples of how to use this command, see [Examples](#BKMK_examples).

> [!NOTE]
> In Windows Server 2008 R2, Terminal Services was renamed Remote Desktop Services. To find out what's new in the latest version, see [What’s New in Remote Desktop Services in Windows Server 2012](http://technet.microsoft.com/library/hh831527) in the Windows Server TechNet Library.

## Syntax

```
query session [<SessionName> | <UserName> | <SessionID>] [/server:<ServerName>] [/mode] [/flow] [/connect] [/counter]
```

## Parameters

|Parameter|Description|
|-------------|---------------|
|<SessionName>|Specifies the name of the session that you want to query.|
|<UserName>|Specifies the name of the user whose sessions you want to query.|
|<SessionID>|Specifies the ID of the session that you want to query.|
|\/server:<ServerName>|Identifies the RD Session Host server to query. The default is the current server.|
|\/mode|Displays current line settings.|
|\/flow|Displays current flow\-control settings.|
|\/connect|Displays current connect settings.|
|\/counter|Displays current counters information, including the total number of sessions created, disconnected, and reconnected.|
|\/?|Displays help at the command prompt.|

## Remarks

-   A user can always query the session to which the user is currently logged on. To query other sessions, the user must have Query Information special access permission.

-   If you do not specify a session by using <*SessionName*>, <*UserName*>, or <*SessionID*>, **query session** displays information about all active sessions in the system.

-   When **query session** returns information, a greater than \(>\) symbol is displayed before the current session. Following is sample output for **query session**:

    ```
    C:\>query session
     SESSIONNAME    USERNAME       ID STATE  TYPE   DEVICE
    >console        Administrator1  0 active wdcon
     rdp-tcp#1      User1           1 active wdtshare
     rdp-tcp                        2 listen wdtshare
                                    4 idle
                                    5 idle
    ```

    The greater than \(>\) symbol indicates the current session. SESSIONNAME specifies the name assigned to the session. USERNAME indicates the user name of the user connected to the session. STATE provides information about the current state of the session. TYPE indicates the session type. DEVICE, which is not present for the console or network\-connected sessions, is the device name assigned to the session. The comment following session information is from the session profile. Any sessions in which the initial state is configured as DISABLED do not show up in the **query session** list until they are enabled.

## <a name="BKMK_examples"></a>Examples

-   To display information about all active sessions on server SERVER2, type:

    ```
    query session /server:SERVER2
    ```

-   To display information about active session MODEM02, type:

    ```
    query session MODEM02
    ```

#### Additional references
[Command-Line Syntax Key](../Command-Line-Syntax-Key.md)

[Query](../Query.md)

[Remote Desktop Services &#40;Terminal Services&#41; Command Reference](../commands-by-server-role/Remote-Desktop-Services--Terminal-Services--Command-Reference.md)

