---
title: "Tsk.EarnedValueMethod"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Tsk 字段。确定应使用“完成”还是“实际完成”字段来计算已完成工作预算成本（BCWP）"
type: docs
weight: 350
url: /zh/net/aspose.tasks/tsk/earnedvaluemethod/
---
## Tsk.EarnedValueMethod field

确定应使用“完成百分比”还是“实际完成百分比”字段来计算已完成工作预算成本（BCWP）。

```csharp
public static readonly Key<EarnedValueMethodType, TaskKey> EarnedValueMethod;
```

## 示例

展示如何读取/写入 Tsk.EarnedValueMethod 属性。

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.EarnedValueMethod, EarnedValueMethodType.PercentComplete);

Console.WriteLine("Earned Value Method: " + task.Get(Tsk.EarnedValueMethod));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [EarnedValueMethodType](../../earnedvaluemethodtype/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


