---
title: "Prj.NewTasksEstimated"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。确定是否默认显示估计持续时间"
type: docs
weight: 570
url: /zh/net/aspose.tasks/prj/newtasksestimated/
---
## Prj.NewTasksEstimated field

确定是否默认显示估计工期。

```csharp
public static readonly Key<NullableBool, PrjKey> NewTasksEstimated;
```

## 示例

展示如何读取/写入 Prj.NewTasksEstimated 属性。

```csharp
var project = new Project();

project.Set(Prj.NewTasksEstimated, true);

Console.WriteLine("New Tasks Estimated: " + project.Get(Prj.NewTasksEstimated));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


