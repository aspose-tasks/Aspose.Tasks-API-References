---
title: "Project.ResourceAssignments"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Project 属性。获取 ResourceAssignmentCollection 对象"
type: docs
weight: 750
url: /zh/net/aspose.tasks/project/resourceassignments/
---
## Project.ResourceAssignments property

获取 ResourceAssignmentCollection 对象。

```csharp
public ResourceAssignmentCollection ResourceAssignments { get; }
```

## 示例

展示如何使用资源分配。

```csharp
var project = new Project();

// 添加新任务和资源
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Rsc");

// 将资源分配到所需任务
project.ResourceAssignments.Add(task, resource);
```

### 另见

* class [ResourceAssignmentCollection](../../resourceassignmentcollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


