---
title: "ResourceUsageViewFieldCollection.ToList"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ResourceUsageViewFieldCollection 方法。将 ResourceUsageViewFieldCollection 类的实例转换为包含 ResourceUsageViewField 类实例的列表"
type: docs
weight: 20
url: /zh/net/aspose.tasks/resourceusageviewfieldcollection/tolist/
---
## ResourceUsageViewFieldCollection.ToList method

将 [`ResourceUsageViewFieldCollection`](../) 类的实例转换为包含 [`ResourceUsageViewField`](../../resourceusageviewfield/) 类实例的列表。

```csharp
public IList<ResourceUsageViewField> ToList()
```

### 返回值

该 [`ResourceUsageViewFieldCollection`](../) 类的实例已转换为包含 [`ResourceUsageViewField`](../../resourceusageviewfield/) 类实例的列表。

## 示例

展示如何使用 ResourceUsageView 实例的字段集合。

```csharp
var project = new Project(DataDir + "ResourceUsageView.mpp");

var view = (ResourceUsageView)project.Views.ToList()[2];
foreach (var field in view.FieldCollection)
{
    Console.WriteLine("Field: " + field);
}

// 可以将集合转换为 ResourceUsageViewField 列表
IList<ResourceUsageViewField> fields = view.FieldCollection.ToList();
foreach (var field in fields)
{
    Console.WriteLine("Field (from the list): " + field);
}
```

### 另见

* enum [ResourceUsageViewField](../../resourceusageviewfield/)
* class [ResourceUsageViewFieldCollection](../)
* namespace [Aspose.Tasks](../../resourceusageviewfieldcollection/)
* assembly [Aspose.Tasks](../../../)


