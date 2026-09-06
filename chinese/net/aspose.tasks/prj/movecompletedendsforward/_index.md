---
title: "Prj.MoveCompletedEndsForward"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。确定已完成任务的结束时间（这些任务原计划在状态日期前完成但实际开始较晚）是否应上移至状态日期"
type: docs
weight: 500
url: /zh/net/aspose.tasks/prj/movecompletedendsforward/
---
## Prj.MoveCompletedEndsForward field

确定计划在状态日期之前完成但实际稍后开始的已完成任务部分的结束时间是否应提前至状态日期。

```csharp
public static readonly Key<NullableBool, PrjKey> MoveCompletedEndsForward;
```

## 示例

展示如何读取/写入 Prj.MoveCompletedEndsForward 属性。

```csharp
var project = new Project();

project.Set(Prj.MoveCompletedEndsForward, true);

Console.WriteLine("Move Completed Ends Forward: " + project.Get(Prj.MoveCompletedEndsForward));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


