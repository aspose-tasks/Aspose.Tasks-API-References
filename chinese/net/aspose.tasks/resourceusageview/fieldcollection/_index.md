---
title: "ResourceUsageView.FieldCollection"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ResourceUsageView 属性。获取此 ResourceUsageView 的 ResourceUsageViewFieldCollection 对象。"
type: docs
weight: 10
url: /zh/net/aspose.tasks/resourceusageview/fieldcollection/
---
## ResourceUsageView.FieldCollection property

获取此 ResourceUsageView 的 [`ResourceUsageViewFieldCollection`](../../resourceusageviewfieldcollection/) 对象。

```csharp
public ResourceUsageViewFieldCollection FieldCollection { get; }
```

## 示例

显示如何读取资源使用视图字段。

```csharp
var project = new Project(DataDir + "ResourceUsageView.mpp");

var view = (ResourceUsageView)project.Views.ToList()[2];
foreach (var field in view.FieldCollection)
{
    Console.WriteLine("Field: " + field);
}
```

### 另见

* class [ResourceUsageViewFieldCollection](../../resourceusageviewfieldcollection/)
* class [ResourceUsageView](../)
* namespace [Aspose.Tasks](../../resourceusageview/)
* assembly [Aspose.Tasks](../../../)


