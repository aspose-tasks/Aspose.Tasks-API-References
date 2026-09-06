---
title: "类 CustomProjectPropertyCollection"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Properties.CustomProjectPropertyCollection 类。表示自定义项目属性的集合"
type: docs
weight: 1550
url: /zh/net/aspose.tasks.properties/customprojectpropertycollection/
---
## CustomProjectPropertyCollection class

表示自定义项目属性的集合。

```csharp
public sealed class CustomProjectPropertyCollection : PropertyKeyedCollection<CustomProjectProperty>
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [CustomProjectPropertyCollection](customprojectpropertycollection/)() | 初始化 `CustomProjectPropertyCollection` 类的新实例。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [Count](../../aspose.tasks.properties/propertykeyedcollection-1/count/) { get; } |  |
| override [IsReadOnly](../../aspose.tasks.properties/customprojectpropertycollection/isreadonly/) { get; } | 获取一个值，指示此集合是否为只读；否则为 false。 |
| [Item](../../aspose.tasks.properties/propertykeyedcollection-1/item/) { get; } |  |
| [Names](../../aspose.tasks.properties/propertykeyedcollection-1/names/) { get; } |  |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Add](../../aspose.tasks.properties/propertykeyedcollection-1/add/)(CustomProjectProperty) |  |
| [Add](../../aspose.tasks.properties/customprojectpropertycollection/add/#add)(string, bool) | 创建一个新的自定义属性。 |
| [Add](../../aspose.tasks.properties/customprojectpropertycollection/add/#add_2)(string, DateTime) | 创建一个新的自定义属性。 |
| [Add](../../aspose.tasks.properties/customprojectpropertycollection/add/#add_1)(string, double) | 创建一个新的自定义属性。 |
| [Add](../../aspose.tasks.properties/customprojectpropertycollection/add/#add_3)(string, string) | 创建一个新的自定义属性。 |
| [Clear](../../aspose.tasks.properties/customprojectpropertycollection/clear/)() | 清除 PropertyCollection。 |
| [Contains](../../aspose.tasks.properties/propertykeyedcollection-1/contains/)(string) |  |
| [Remove](../../aspose.tasks.properties/customprojectpropertycollection/remove/)(string) | 从集合中移除具有指定名称的属性。 |

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

* class [PropertyKeyedCollection&lt;T&gt;](../propertykeyedcollection-1/)
* class [CustomProjectProperty](../customprojectproperty/)
* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


