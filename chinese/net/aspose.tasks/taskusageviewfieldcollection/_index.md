---
title: "类 TaskUsageViewFieldCollection"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.TaskUsageViewFieldCollection 类。表示 TaskUsageViewField 值的集合"
type: docs
weight: 2500
url: /zh/net/aspose.tasks/taskusageviewfieldcollection/
---
## TaskUsageViewFieldCollection class

表示 [`TaskUsageViewField`](../taskusageviewfield/) 值的集合。

```csharp
public class TaskUsageViewFieldCollection : IList<TaskUsageViewField>
```

## 方法

| 名称 | 描述 |
| --- | --- |
| [GetEnumerator](../../aspose.tasks/taskusageviewfieldcollection/getenumerator/)() | 返回此集合的枚举器。 |
| [ToList](../../aspose.tasks/taskusageviewfieldcollection/tolist/)() | 返回包含此集合中所有项目的列表。 |

## 示例

展示如何使用 TaskUsageView 实例的字段集合。

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = (TaskUsageView)project.Views.ToList()[2];
foreach (var field in view.FieldCollection)
{
    Console.WriteLine("Field: " + field);
}

// 可以将集合转换为 TaskUsageViewField 列表
IList<TaskUsageViewField> fields = view.FieldCollection.ToList();
foreach (var field in fields)
{
    Console.WriteLine("Field (from the list): " + field);
}
```

### 另见

* enum [TaskUsageViewField](../taskusageviewfield/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


