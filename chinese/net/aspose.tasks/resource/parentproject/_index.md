---
title: "Resource.ParentProject"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Resource 属性。获取此容器的父项目"
type: docs
weight: 600
url: /zh/net/aspose.tasks/resource/parentproject/
---
## Resource.ParentProject property

获取此容器的父项目。

```csharp
public Project ParentProject { get; }
```

## 示例

展示如何使用资源的父项目。

```csharp
var project = new Project();
var resource = project.Resources.Add("Resource");

// 通过使用默认项目工作时间单位类型为资源设置工作。
resource.Set(Rsc.Work, resource.ParentProject.GetWork(1));

Console.WriteLine(resource.Get(Rsc.Work));
```

### 另见

* class [Project](../../project/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


