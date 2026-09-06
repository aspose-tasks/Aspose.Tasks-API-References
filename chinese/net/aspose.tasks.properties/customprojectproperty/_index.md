---
title: "类 CustomProjectProperty"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Properties.CustomProjectProperty 类。表示自定义属性"
type: docs
weight: 1540
url: /zh/net/aspose.tasks.properties/customprojectproperty/
---
## CustomProjectProperty class

表示自定义属性。

```csharp
public sealed class CustomProjectProperty : Property
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Name](../../aspose.tasks.properties/property/name/) { get; } | 获取属性的名称。 |
| [Type](../../aspose.tasks.properties/customprojectproperty/type/) { get; } | 获取属性的类型。 |
| [Value](../../aspose.tasks.properties/property/value/) { get; set; } | 获取或设置属性的值。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| override [ToString](../../aspose.tasks.properties/property/tostring/)() | 以字符串形式返回属性值。 |

## 示例

展示如何使用自定义项目属性集合。

```csharp
var project = new Project(DataDir + "ReadProjectInfo.mpp");

Console.WriteLine("Is custom properties collection read-only?: " + project.CustomProps.IsReadOnly);

// 让我们添加新的自定义属性
// 集合支持 Boolean、DateTime、Double、String 类型
project.CustomProps.Add("IsEnterprise", true);
project.CustomProps.Add("Project Start Date", new DateTime(2020, 4, 16, 8, 0, 0));
project.CustomProps.Add("Precision", 10d);
project.CustomProps.Add("Custom Name", "MyProject");

// 自定义属性可通过类型化集合访问
Console.WriteLine("Count of custom properties: " + project.CustomProps.Count);
foreach (var property in project.CustomProps)
{
    Console.WriteLine(property.Type);
    Console.WriteLine(property.Name);
    Console.WriteLine(property.Value);
    Console.WriteLine();
}

// 获取自定义属性值
Console.WriteLine("Custom Name: " + project.CustomProps["Custom Name"]);

// 遍历自定义属性的名称
foreach (var propsName in project.CustomProps.Names)
{
    Console.WriteLine("Name: " + propsName);
    Console.WriteLine();
}

// 可以通过字符串键删除值
if (project.CustomProps.Contains("Custom Name"))
{
    project.CustomProps.Remove("Custom Name");
}

// 或者可以完全清除集合
project.CustomProps.Clear();
```

### 另见

* class [Property](../property/)
* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


