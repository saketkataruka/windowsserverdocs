---
title: Attach additional stations to your Windows MultiPoint Server 2012 computer
ms.custom: na
ms.date: 07/22/2016
ms.prod: multipoint-server-2012
ms.reviewer: na
ms.suite: na
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: d78ebf4e-0968-4014-9a42-9f75cc50cb52
author: lizap
manager: jwhit
---
# Attach additional stations to your Windows MultiPoint Server 2012 computer
In your MultiPoint Server environment, your users use stations to connect to the MultiPoint Server computer and do their work. The stations are the user endpoints for connecting to the computer running [!INCLUDE[win8_server_multipoint_2](../../../compute/remote-desktop-services/multipoint-1/includes/win8_server_multipoint_2_md.md)].  
  
MultiPoint Server supports three types of station:  
  
-   Direct\-video\-connected stations  
  
-   USB zero client\-connected stations \(and USB over Ethernet zero client connected stations\)  
  
-   RDP\-over\-LAN connected stations  
  
The classifications are based on a station’s hardware and the type of connection that it uses. You can mix and match connection types for your stations. The only requirement is that the primary station \(which you installed earlier\) must be a direct\-video\-connected station. For more information about station setups, see [MultiPoint Server Stations](../../../compute/remote-desktop-services/multipoint-1/MultiPoint-Server-Stations.md) \(http:\/\/technet.microsoft.com\/library\/jj916411.aspx\).  
  
For instructions that explain how to set up each type of station, see the following:  
  
-   [Set up a direct-video-connected station in Windows MultiPoint Server 2012](../../../compute/remote-desktop-services/multipoint-1/Set-up-a-direct-video-connected-station-in-Windows-MultiPoint-Server-2012.md)  
  
-   [Set up a USB zero client-connected station in Windows MultiPoint Server 2012](../../../compute/remote-desktop-services/multipoint-1/Set-up-a-USB-zero-client-connected-station-in-Windows-MultiPoint-Server-2012.md)  
  
-   [Set up an RDP-over-LAN connected station in Windows MultiPoint Server 2012](../../../compute/remote-desktop-services/multipoint-1/Set-up-an-RDP-over-LAN-connected-station-in-Windows-MultiPoint-Server-2012.md)  
  
For a detailed comparison of station types, see [Station type comparison](assetId:///a8a25e40-e3a5-4121-ac23-77e7c5ac358f#BKMK_StationTypeComparison) in [MultiPoint Server Stations](../../../compute/remote-desktop-services/multipoint-1/MultiPoint-Server-Stations.md) \(http:\/\/technet.microsoft.com\/library\/jj916411.aspx\).  
  
> [!NOTE]  
> -   The procedures for attaching stations do not describe how to set up intermediate hubs or downstream hubs. For information about where to install these hubs, see [MultiPoint Server Stations](../../../compute/remote-desktop-services/multipoint-1/MultiPoint-Server-Stations.md).  
> -   In some cases, you might need to create station virtual desktops, which run in virtual machines. For example, you use applications that cannot be installed on Windows Server or applications that will not run multiple instances on the same host computer. For more information, see [Create Windows 7 or Windows 8 Enterprise virtual desktops for stations](../../../compute/remote-desktop-services/multipoint-1/Create-Windows-7-or-Windows-8-Enterprise-virtual-desktops-for-stations.md).  
  
> [!TIP]  
> It is useful to create your stations in the order of their physical locations so that they are identified sequentially in MultiPoint Server. If you later want to change the name of a station, you can do that in MultiPoint Manager. For more information, see Remap all stations in MultiPoint Server Help and Support.  
  