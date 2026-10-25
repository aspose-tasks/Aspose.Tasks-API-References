---
title: "Prj.WorkFormat"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。用于显示任务持续时间的格式"
type: docs
weight: 790
url: /zh/net/aspose.tasks/prj/workformat/
---
## Prj.WorkFormat field

用于显示任务持续时间的格式。

```csharp
public static readonly Key<TimeUnitType, PrjKey> WorkFormat;
```

## 示例

展示如何使用默认工作格式获取持续时间。

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

Console.WriteLine("Project's work format: " + project.Get(Prj.WorkFormat));

// 使用项目的默认工作格式创建工作值
var work = project.GetWork(2);
Console.WriteLine("Work: " + work.TimeSpan);
Console.WriteLine("Time unit: " + work.TimeUnit);
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TimeUnitType](../../timeunittype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


