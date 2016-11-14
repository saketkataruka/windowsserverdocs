---
title: Audit Filtering Platform Packet Drop
description: "Windows Server Security"
ms.custom: na
ms.prod: windows-server-threshold
ms.reviewer: na
ms.suite: na
ms.technology: security-auditing
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: f207f4e8-d0f7-4234-acf8-a982bfd7d776
author: coreyp-at-msft
ms.author: coreyp
manager: dongill
ms.date: 10/12/2016
---
# Audit Filtering Platform Packet Drop

>Applies To: Windows Server&reg; 2016, Windows Server&reg; 2012 R2, Windows Server&reg; 2012

This topic for the IT professional describes the Advanced Security Audit policy setting, **Audit Filtering Platform Packet Drop**, which determines whether the operating system generates audit events when packets are dropped by the Windows Filtering Platform.

Windows Filtering Platform (WFP) was introduced in Windows Server 2008 and Windows Vista to enable independent software vendors (ISVs) to filter and modify TCP/IP packets, monitor or authorize connections, filter Internet Protocol security (IPsec)-protected traffic, and filter remote procedure calls (RPCs).

A high rate of dropped packets may indicate that there have been attempts to gain unauthorized access to computers on your network.

Event volume: High

Default setting: Not configured

If this policy setting is configured, the following events appear on computers running the supported versions of the Windows operating system as designated in the  **Applies to** list at the beginning of this topic, in addition to Windows Server 2008 and Windows Vista.

|Event ID|Event message|
|------|---------|
|5152|The Windows Filtering Platform blocked a packet.|
|5153|A more restrictive Windows Filtering Platform filter has blocked a packet.|

## Related resource
[Advanced Security Audit Policy Settings](../advanced-security-audit-policy-settings.md)

