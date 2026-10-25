---
title: "枚举 ApplicationInfo"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.ApplicationInfo 枚举。指定创建文件时的项目版本。"
type: docs
weight: 10
url: /zh/net/aspose.tasks/applicationinfo/
---
## ApplicationInfo enumeration

指定创建文件的项目版本。

```csharp
public enum ApplicationInfo
```

### 值

| 名称 | 值 | 描述 |
| --- | --- | --- |
| Undefined | `0` | 无法定义。 |
| MSP2000 | `1` | 文件创建于 Microsoft Project 2000/2002。 |
| MSP2003 | `2` | 文件创建于 Microsoft Project 2003。 |
| MSP2007 | `3` | 文件创建于 Microsoft Project 2007。 |
| MSP2010 | `4` | 文件创建于 Microsoft Project 2010。 |
| MSP2013 | `5` | 文件创建于 Microsoft Project 2013。 |
| MSP2016 | `6` | 文件创建于 Microsoft Project 2016。 |

## 示例

展示如何检查项目应用程序信息。

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### 另见

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


