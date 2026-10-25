---
title: "Resource.Assignments"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Resource 属性。获取此对象的资源分配集合"
type: docs
weight: 120
url: /zh/net/aspose.tasks/resource/assignments/
---
## Resource.Assignments property

获取此对象的资源分配集合。

```csharp
public ResourceAssignmentCollection Assignments { get; }
```

## 示例

展示如何读取资源的分配。

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

foreach (var resource in project.Resources)
{
    foreach (var assignment in resource.Assignments)
    {
        Console.WriteLine("Assignment UID: " + assignment.Get(Asn.Uid));
        Console.WriteLine("Assignment's task name: " + assignment.Get(Asn.Task).Get(Tsk.Name));
    }
}
```

### 另见

* class [ResourceAssignmentCollection](../../resourceassignmentcollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


