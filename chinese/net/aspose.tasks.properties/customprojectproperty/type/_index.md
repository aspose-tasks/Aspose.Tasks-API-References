---
title: "CustomProjectProperty.Type"
second_title: "Aspose.Tasks for .NET API 参考"
description: "CustomProjectProperty 属性。获取属性的类型。"
type: docs
weight: 10
url: /zh/net/aspose.tasks.properties/customprojectproperty/type/
---
## CustomProjectProperty.Type property

获取属性的类型。

```csharp
public CustomPropertyType Type { get; }
```

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

* enum [CustomPropertyType](../../custompropertytype/)
* class [CustomProjectProperty](../)
* namespace [Aspose.Tasks.Properties](../../customprojectproperty/)
* assembly [Aspose.Tasks](../../../)


