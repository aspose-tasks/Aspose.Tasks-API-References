---
title: Enum FileFormat
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.FileFormat enum. Specifies the projects file format
type: docs
weight: 590
url: /net/aspose.tasks/fileformat/
---
## FileFormat enumeration

Specifies the project's file format.

```csharp
public enum FileFormat
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Undefined | `0` | Can not be defined. |
| P6XML | `1` | Represents Primavera P6 XML format. |
| XML | `2` | Microsoft Project XML format. |
| MPP8 | `3` | Microsoft Project 2000 format. |
| MPP9 | `4` | Microsoft Project 2003 format. |
| MPP12 | `5` | Microsoft Project 2007 format. |
| MPP14 | `6` | Microsoft Project 2010 format. |
| MPT9 | `7` | Microsoft Project 2003 template format. |
| MPT12 | `8` | Microsoft Project 2007 template format. |
| MPT14 | `9` | Microsoft Project 2010 (2013) template format. |
| MPX | `10` | Mpx file format |
| XER | `11` | Represents Primavera XER format |
| HTML | `12` | Represents HTML format |
| ProjectServer | `13` | Project was read from Project Server or Project Online |

## Examples

Shows how to read check project file format.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


