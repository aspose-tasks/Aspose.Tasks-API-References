---
title: "类 ResourceUsageViewFieldCollection"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.ResourceUsageViewFieldCollection 类。表示 ResourceUsageViewField 值的集合"
type: docs
weight: 1830
url: /zh/net/aspose.tasks/resourceusageviewfieldcollection/
---
## ResourceUsageViewFieldCollection class

表示一个 [`ResourceUsageViewField`](../resourceusageviewfield/) 值的集合。

```csharp
public class ResourceUsageViewFieldCollection : IList<ResourceUsageViewField>
```

## 方法

| 名称 | 描述 |
| --- | --- |
| [GetEnumerator](../../aspose.tasks/resourceusageviewfieldcollection/getenumerator/)() | 返回此集合的枚举器。 |
| [ToList](../../aspose.tasks/resourceusageviewfieldcollection/tolist/)() | 将 `ResourceUsageViewFieldCollection` 类的实例转换为包含 [`ResourceUsageViewField`](../resourceusageviewfield/) 类实例的列表。 |

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

* enum [ResourceUsageViewField](../resourceusageviewfield/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


