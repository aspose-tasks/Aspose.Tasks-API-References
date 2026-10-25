---
title: "ResourceAssignment.Guid"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ResourceAssignment 属性。获取或设置此分配的唯一标识符"
type: docs
weight: 290
url: /zh/net/aspose.tasks/resourceassignment/guid/
---
## ResourceAssignment.Guid property

获取或设置此分配的唯一标识符。

```csharp
public Guid? Guid { get; set; }
```

## 示例

展示如何读取资源分配的 GUID。

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var assignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine(assignment.Guid);
```

### 另见

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


