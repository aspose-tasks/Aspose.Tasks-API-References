---
title: "ResourceUsageViewFieldCollection.GetEnumerator"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ResourceUsageViewFieldCollection 方法。返回此集合的枚举器"
type: docs
weight: 10
url: /zh/net/aspose.tasks/resourceusageviewfieldcollection/getenumerator/
---
## ResourceUsageViewFieldCollection.GetEnumerator method

返回此集合的枚举器。

```csharp
public IEnumerator<ResourceUsageViewField> GetEnumerator()
```

### 返回值

此集合的枚举器。

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


