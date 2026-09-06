---
title: "TaskUsageViewFieldCollection.GetEnumerator"
second_title: "Aspose.Tasks for .NET API 参考"
description: "TaskUsageViewFieldCollection 方法。返回此集合的枚举器。"
type: docs
weight: 10
url: /zh/net/aspose.tasks/taskusageviewfieldcollection/getenumerator/
---
## TaskUsageViewFieldCollection.GetEnumerator method

返回此集合的枚举器。

```csharp
public IEnumerator<TaskUsageViewField> GetEnumerator()
```

### 返回值

此集合的枚举器。

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


