---
title: "枚举 FileFormat"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.FileFormat 枚举。指定项目文件格式"
type: docs
weight: 590
url: /zh/net/aspose.tasks/fileformat/
---
## FileFormat enumeration

指定项目的文件格式。

```csharp
public enum FileFormat
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Undefined | `0` | 无法定义。 |
| P6XML | `1` | 表示 Primavera P6 XML 格式。 |
| XML | `2` | Microsoft Project XML 格式。 |
| MPP8 | `3` | Microsoft Project 2000 格式。 |
| MPP9 | `4` | Microsoft Project 2003 格式。 |
| MPP12 | `5` | Microsoft Project 2007 格式。 |
| MPP14 | `6` | Microsoft Project 2010 格式。 |
| MPT9 | `7` | Microsoft Project 2003 模板格式。 |
| MPT12 | `8` | Microsoft Project 2007 模板格式。 |
| MPT14 | `9` | Microsoft Project 2010（2013）模板格式。 |
| MPX | `10` | Mpx 文件格式 |
| XER | `11` | 表示 Primavera XER 格式 |
| HTML | `12` | 表示 HTML 格式 |
| ProjectServer | `13` | 项目是从 Project Server 或 Project Online 读取的 |

## 示例

展示如何读取检查项目文件格式。

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


