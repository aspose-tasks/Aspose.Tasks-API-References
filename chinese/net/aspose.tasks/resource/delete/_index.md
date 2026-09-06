---
title: "Resource.Delete"
second_title: "Aspose.Tasks for .NET API 参考"
description: "资源方法。删除项目中的资源及其分配"
type: docs
weight: 810
url: /zh/net/aspose.tasks/resource/delete/
---
## Resource.Delete method

从项目中删除资源及其分配。

```csharp
public void Delete()
```

## 示例

展示如何删除资源。

```csharp
var project = new Project(DataDir + "Baselines2010.mpp");

var resource = project.Resources.GetById(1);

Console.WriteLine("Number of resources (before): " + project.Resources.Count);

// 删除资源
resource.Delete();

Console.WriteLine("Number of resources (after): " + project.Resources.Count);
```

### 另见

* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


