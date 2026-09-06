---
title: "Prj.MoveRemainingStartsForward"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。确定是否应将计划稍后开始的任务剩余部分的起始时间提前至状态日期"
type: docs
weight: 520
url: /zh/net/aspose.tasks/prj/moveremainingstartsforward/
---
## Prj.MoveRemainingStartsForward field

确定是否应将计划稍后开始的任务剩余部分的开始时间提前至状态日期。

```csharp
public static readonly Key<NullableBool, PrjKey> MoveRemainingStartsForward;
```

## 示例

展示如何读取/写入 Prj.MoveRemainingStartsForward 属性。

```csharp
var project = new Project();

project.Set(Prj.MoveRemainingStartsForward, true);

Console.WriteLine("Move Remaining Starts Forward: " + project.Get(Prj.MoveRemainingStartsForward));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


