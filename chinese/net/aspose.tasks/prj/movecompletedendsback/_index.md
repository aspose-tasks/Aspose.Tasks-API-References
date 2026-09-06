---
title: "Prj.MoveCompletedEndsBack"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。确定是否应将计划在状态日期之后开始但实际提前开始的已完成任务部分的结束时间移回状态日期"
type: docs
weight: 490
url: /zh/net/aspose.tasks/prj/movecompletedendsback/
---
## Prj.MoveCompletedEndsBack field

确定计划在状态日期之后开始但实际提前开始的已完成任务部分的结束时间是否应移回状态日期。

```csharp
public static readonly Key<NullableBool, PrjKey> MoveCompletedEndsBack;
```

## 示例

展示如何读取/写入 Prj.MoveCompletedEndsBack 属性。

```csharp
var project = new Project();

project.Set(Prj.MoveCompletedEndsBack, true);

Console.WriteLine("Move Completed Ends Back: " + project.Get(Prj.MoveCompletedEndsBack));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


