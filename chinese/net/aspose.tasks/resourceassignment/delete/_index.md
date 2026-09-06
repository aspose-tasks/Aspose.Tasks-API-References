---
title: "ResourceAssignment.Delete"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ResourceAssignment 方法。 从项目分配集合中删除资源分配"
type: docs
weight: 680
url: /zh/net/aspose.tasks/resourceassignment/delete/
---
## ResourceAssignment.Delete method

从项目分配集合中删除资源分配。

```csharp
public void Delete()
```

## 示例

展示如何删除资源分配。

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var resourceAssignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine("Assignment count (before): {0}", project.ResourceAssignments.Count);

resourceAssignment.Delete();

Console.WriteLine("Assignment count (after): {0}", project.ResourceAssignments.Count);
```

### 另见

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


