---
title: "FieldHelper.GetDefaultTaskFieldTitle"
second_title: "Aspose.Tasks for .NET API 参考"
description: "FieldHelper 方法。 返回特定任务字段的默认标题"
type: docs
weight: 20
url: /zh/net/aspose.tasks.util/fieldhelper/getdefaulttaskfieldtitle/
---
## FieldHelper.GetDefaultTaskFieldTitle method

返回特定任务字段的默认标题。

```csharp
public static string GetDefaultTaskFieldTitle(TaskKey taskKey)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| taskKey | TaskKey | 用于获取默认标题的任务字段。 |

### 返回值

如果该字段可以在 MS Project 视图中显示，则返回特定任务字段的默认标题；否则返回 null。

## 示例

展示如何获取特定任务字段的默认标题。

```csharp
Console.WriteLine("Title for Tsk.ActualCost: " + FieldHelper.GetDefaultTaskFieldTitle(Tsk.ActualCost.KeyType));
Console.WriteLine("Title for Tsk.PercentWorkComplete: " + FieldHelper.GetDefaultTaskFieldTitle(Tsk.PercentWorkComplete.KeyType));
```

### 另见

* enum [TaskKey](../../../aspose.tasks/taskkey/)
* class [FieldHelper](../)
* namespace [Aspose.Tasks.Util](../../fieldhelper/)
* assembly [Aspose.Tasks](../../../)


