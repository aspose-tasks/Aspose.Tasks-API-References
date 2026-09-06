---
title: "TaskUsageView.FieldCollection"
second_title: "Aspose.Tasks for .NET API 参考"
description: "TaskUsageView 属性。获取此 TaskUsageView 的 TaskUsageViewFieldCollection 对象"
type: docs
weight: 10
url: /zh/net/aspose.tasks/taskusageview/fieldcollection/
---
## TaskUsageView.FieldCollection property

获取此 TaskUsageView 的 [`TaskUsageViewFieldCollection`](../../taskusageviewfieldcollection/) 对象。

```csharp
public TaskUsageViewFieldCollection FieldCollection { get; }
```

## 示例

展示如何读取任务使用视图字段。

```csharp
var project = new Project(DataDir + "TaskUsageView.mpp");

var view = (TaskUsageView)project.Views.ToList()[2];
foreach (var field in view.FieldCollection)
{
    Console.WriteLine("Field: " + field);
}
```

### 另见

* class [TaskUsageViewFieldCollection](../../taskusageviewfieldcollection/)
* class [TaskUsageView](../)
* namespace [Aspose.Tasks](../../taskusageview/)
* assembly [Aspose.Tasks](../../../)


