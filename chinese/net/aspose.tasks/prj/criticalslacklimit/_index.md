---
title: "Prj.CriticalSlackLimit"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。如果总浮动小于或等于此天数，MS Project 将任务视为关键任务"
type: docs
weight: 140
url: /zh/net/aspose.tasks/prj/criticalslacklimit/
---
## Prj.CriticalSlackLimit field

如果总浮动小于或等于此天数，MS Project 将任务视为关键任务。

```csharp
public static readonly Key<int, PrjKey> CriticalSlackLimit;
```

## 示例

展示如何读取/写入 Prj.CriticalSlackLimit 属性。

```csharp
var project = new Project();

project.Set(Prj.CriticalSlackLimit, 2);

Console.WriteLine("Critical Slack Limit: " + project.Get(Prj.CriticalSlackLimit));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


