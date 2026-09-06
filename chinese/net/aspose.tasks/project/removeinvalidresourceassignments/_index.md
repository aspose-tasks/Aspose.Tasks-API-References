---
title: "Project.RemoveInvalidResourceAssignments"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Project 方法。消除项目资源分配列表中的无效资源分配。"
type: docs
weight: 1170
url: /zh/net/aspose.tasks/project/removeinvalidresourceassignments/
---
## Project.RemoveInvalidResourceAssignments method

从项目资源分配列表中消除无效的资源分配。

```csharp
public void RemoveInvalidResourceAssignments()
```

## 备注

MS Project 为每个任务创建一个空的资源分配。调用该方法将其移除。

## 示例

展示如何移除无效分配。

```csharp
var project = new Project(DataDir + "InvalidResourceAssignments.mpp");
var invalid = 0;

// ReSharper disable once LoopCanBeConvertedToQuery //ExSkip
foreach (var ra in project.ResourceAssignments)
{
    if (ra.Get(Asn.Resource) == null)
    {
        invalid++;
    }
}

Console.WriteLine("Count of invalid assignments (before): " + invalid);

// 移除无效分配
project.RemoveInvalidResourceAssignments();

Console.WriteLine("Count of invalid assignments (after): " + invalid);
```

### 另见

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


