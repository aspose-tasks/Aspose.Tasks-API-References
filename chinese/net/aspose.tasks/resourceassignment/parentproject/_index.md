---
title: "ResourceAssignment.ParentProject"
second_title: "Aspose.Tasks for .NET API 参考"
description: "ResourceAssignment 属性。获取此分配的父项目"
type: docs
weight: 420
url: /zh/net/aspose.tasks/resourceassignment/parentproject/
---
## ResourceAssignment.ParentProject property

获取此分配的父项目。

```csharp
public Project ParentProject { get; }
```

## 示例

展示如何使用资源分配的父项目。

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");
var resource = project.Resources.Add("Resource");
var resourceAssignment = project.ResourceAssignments.Add(task, resource);

// 通过使用默认项目时间单位类型来设置分配的持续时间。
resourceAssignment.Set(Asn.Work, resource.ParentProject.GetWork(1));

Console.WriteLine(resourceAssignment.Get(Asn.Work));
```

### 另见

* class [Project](../../project/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


