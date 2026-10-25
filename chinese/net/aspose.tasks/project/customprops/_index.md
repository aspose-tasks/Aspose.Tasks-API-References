---
title: "Project.CustomProps"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Project 属性。获取项目自定义属性集合。"
type: docs
weight: 260
url: /zh/net/aspose.tasks/project/customprops/
---
## Project.CustomProps property

获取项目的自定义属性集合。

```csharp
public CustomProjectPropertyCollection CustomProps { get; }
```

## 示例

展示如何读取项目元属性（已废弃的 API）。

```csharp
var project = new Project(DataDir + "ReadProjectInfo.mpp");

// 自定义属性可通过类型化集合访问
foreach (var property in project.CustomProps)
{
    Console.WriteLine(property.Type);
    Console.WriteLine(property.Name);
    Console.WriteLine(property.Value);
}

// 内置属性可直接使用。
Console.WriteLine(project.BuiltInProps.Author);
Console.WriteLine(project.BuiltInProps.Title);

// 或作为内置属性集合的项。
foreach (var property in project.BuiltInProps)
{
    Console.WriteLine(property.Name);
    Console.WriteLine(property.Value);
}
```

### 另见

* class [CustomProjectPropertyCollection](../../../aspose.tasks.properties/customprojectpropertycollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


