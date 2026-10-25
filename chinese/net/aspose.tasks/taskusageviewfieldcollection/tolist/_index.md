---
title: "TaskUsageViewFieldCollection.ToList"
second_title: "Aspose.Tasks for .NET API 参考"
description: "TaskUsageViewFieldCollection 方法。返回包含此集合所有项目的列表。"
type: docs
weight: 20
url: /zh/net/aspose.tasks/taskusageviewfieldcollection/tolist/
---
## TaskUsageViewFieldCollection.ToList method

返回包含此集合中所有项目的列表。

```csharp
public IList<TaskUsageViewField> ToList()
```

### 返回值

返回包含此集合所有项目的列表。

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

* enum [TaskUsageViewField](../../taskusageviewfield/)
* class [TaskUsageViewFieldCollection](../)
* namespace [Aspose.Tasks](../../taskusageviewfieldcollection/)
* assembly [Aspose.Tasks](../../../)


