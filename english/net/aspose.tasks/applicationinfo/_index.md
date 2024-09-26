---
title: Enum ApplicationInfo
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.ApplicationInfo enum. Specifies the project version where the file was created
type: docs
weight: 10
url: /net/aspose.tasks/applicationinfo/
---
## ApplicationInfo enumeration

Specifies the project version where the file was created.

```csharp
public enum ApplicationInfo
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Undefined | `0` | Can not be defined. |
| MSP2000 | `1` | File was created in Microsoft Project 2000/2002. |
| MSP2003 | `2` | File was created in Microsoft Project 2003. |
| MSP2007 | `3` | File was created in Microsoft Project 2007. |
| MSP2010 | `4` | File was created in Microsoft Project 2010. |
| MSP2013 | `5` | File was created in Microsoft Project 2013. |
| MSP2016 | `6` | File was created in Microsoft Project 2016. |

## Examples

Shows how to check project application info.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


