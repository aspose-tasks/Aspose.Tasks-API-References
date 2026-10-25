---
title: "Prj.MoveRemainingStartsBack"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。确定是否应将计划在状态日期之后开始但实际提前开始的任务剩余部分的起始时间移回状态日期。"
type: docs
weight: 510
url: /zh/net/aspose.tasks/prj/moveremainingstartsback/
---
## Prj.MoveRemainingStartsBack field

确定是否应将计划在状态日期之后开始但实际提前开始的任务剩余部分的开始时间移回状态日期。

```csharp
public static readonly Key<NullableBool, PrjKey> MoveRemainingStartsBack;
```

## 示例

展示如何读取/写入 Prj.MoveRemainingStartsBack 属性。

```csharp
var project = new Project();

project.Set(Prj.MoveRemainingStartsBack, true);

Console.WriteLine("Move Remaining Starts Back: " + project.Get(Prj.MoveRemainingStartsBack));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


