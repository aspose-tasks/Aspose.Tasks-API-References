---
title: "类 PropertyKeyedCollectionT"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.Properties.PropertyKeyedCollection1T 类。属性集合的基类"
type: docs
weight: 1600
url: /zh/net/aspose.tasks.properties/propertykeyedcollection-1/
---
## PropertyKeyedCollection&lt;T&gt; class

属性集合的基类。

```csharp
public abstract class PropertyKeyedCollection<T> : PropertyCollection<T>, ICollection<T>
    where T : Property
```

| 参数 | 描述 |
| --- | --- |
| T | 属性的类型。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [Count](../../aspose.tasks.properties/propertykeyedcollection-1/count/) { get; } | 获取集合中属性的数量。 |
| abstract [IsReadOnly](../../aspose.tasks.properties/propertykeyedcollection-1/isreadonly/) { get; } | 获取一个值，指示此集合是否为只读；否则为 false。 |
| [Item](../../aspose.tasks.properties/propertykeyedcollection-1/item/) { get; } | 获取与指定键关联的属性。 |
| [Names](../../aspose.tasks.properties/propertykeyedcollection-1/names/) { get; } | 获取所有属性名称的集合。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Add](../../aspose.tasks.properties/propertykeyedcollection-1/add/)(T) | 创建一个新的自定义属性。 |
| [Contains](../../aspose.tasks.properties/propertykeyedcollection-1/contains/)(string) | 确定 [`PropertyCollection`](../propertycollection-1/) 是否包含具有指定名称的属性。 |

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

* class [PropertyCollection&lt;T&gt;](../propertycollection-1/)
* class [Property](../property/)
* namespace [Aspose.Tasks.Properties](../../aspose.tasks.properties/)
* assembly [Aspose.Tasks](../../)


