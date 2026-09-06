---
title: "Prj.ShowProjectSummaryTask"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。确定是否在甘特图视图顶部的单行中显示整个项目的汇总信息及其自己的汇总任务条"
type: docs
weight: 640
url: /zh/net/aspose.tasks/prj/showprojectsummarytask/
---
## Prj.ShowProjectSummaryTask field

确定是否在甘特图视图顶部的单行中显示整个项目的汇总信息以及其自己的汇总任务条。

```csharp
public static readonly Key<bool, PrjKey> ShowProjectSummaryTask;
```

## 示例

展示如何读取/写入 Prj.ShowProjectSummaryTask 属性。

```csharp
var project = new Project();

project.Set(Prj.ShowProjectSummaryTask, true);

Console.WriteLine("Show Project Summary Task: " + project.Get(Prj.ShowProjectSummaryTask));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


