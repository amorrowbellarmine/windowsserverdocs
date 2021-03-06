---
title: logman start | stop
description: Reference topic for **** - 

ms.prod: windows-server


ms.technology: manage-windows-commands

ms.topic: article
ms.assetid: a40006a1-876e-474b-aaf1-f365c730deea
author: coreyp-at-msft
ms.author: coreyp
manager: dongill
ms.date: 10/16/2017
---
# logman start | stop

> Applies to: Windows Server (Semi-Annual Channel), Windows Server 2019, Windows Server 2016, Windows Server 2012 R2, Windows Server 2012

start a data collector and set the begin time to manual, or stop a data collector set and set the end time to manual.  

## Syntax  
```  
logman start <[-n] <name>> [options]  
logman stop <[-n] <name>> [options]  
```  
### Parameters  

|     Parameter      |                                 Description                                  |
|--------------------|------------------------------------------------------------------------------|
|         -?         |                       Displays context-sensitive help.                       |
| -s <computer name> |            Perform the command on the specified remote computer.             |
|  -config <value>   |           Specifies the settings file containing command options.            |
|    [-n] <name>     |                          Name of the target object.                          |
|        -ets        | Send commands to Event Trace Sessions directly without saving or scheduling. |
|        -as         |               Perform the requested operation asynchronously.                |

## Examples  
The following command starts the data collector perf_log on the remote computer server_1.  
```  
logman start perf_log -s server_1  
```  
## Additional References  
[logman](logman.md)  
