---
title: "类 OutlineCodeDefinitionCollection"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Aspose.Tasks.OutlineCodeDefinitionCollection 类。表示 OutlineCodeDefinition 对象的集合。"
type: docs
weight: 1180
url: /zh/net/aspose.tasks/outlinecodedefinitioncollection/
---
## OutlineCodeDefinitionCollection class

表示一个 [`OutlineCodeDefinition`](../outlinecodedefinition/) 对象的集合。

```csharp
public class OutlineCodeDefinitionCollection : IList<OutlineCodeDefinition>
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Count](../../aspose.tasks/outlinecodedefinitioncollection/count/) { get; } | 获取此集合中包含的元素数量。 |
| [IsReadOnly](../../aspose.tasks/outlinecodedefinitioncollection/isreadonly/) { get; } | 获取一个值，指示此集合是否为只读；否则为 false。 |
| [Item](../../aspose.tasks/outlinecodedefinitioncollection/item/) { get; set; } | 返回或设置指定索引处的元素。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Add](../../aspose.tasks/outlinecodedefinitioncollection/add/)(OutlineCodeDefinition) | 将指定项添加到此集合中。 |
| [Clear](../../aspose.tasks/outlinecodedefinitioncollection/clear/)() | 从此集合中移除所有项。 |
| [Contains](../../aspose.tasks/outlinecodedefinitioncollection/contains/)(OutlineCodeDefinition) | 如果在此集合中找到指定项则返回 true；否则返回 false。 |
| [CopyTo](../../aspose.tasks/outlinecodedefinitioncollection/copyto/)(OutlineCodeDefinition[], int) | 将此集合的元素复制到指定数组中，从指定的数组索引开始。 |
| [GetEnumerator](../../aspose.tasks/outlinecodedefinitioncollection/getenumerator/)() | 返回此集合的枚举器。 |
| [IndexOf](../../aspose.tasks/outlinecodedefinitioncollection/indexof/)(OutlineCodeDefinition) | 确定此集合中指定项的索引。 |
| [Insert](../../aspose.tasks/outlinecodedefinitioncollection/insert/)(int, OutlineCodeDefinition) | 在指定索引处插入指定项。 |
| [Remove](../../aspose.tasks/outlinecodedefinitioncollection/remove/)(OutlineCodeDefinition) | 从此集合中移除特定对象的第一次出现。 |
| [RemoveAt](../../aspose.tasks/outlinecodedefinitioncollection/removeat/)(int) | 在指定索引处移除一项。 |
| [ToList](../../aspose.tasks/outlinecodedefinitioncollection/tolist/)() | 将此 OutlineCodeDefinitionCollection 对象转换为 [`OutlineCodeDefinition`](../outlinecodedefinition/) 对象的列表。 |

## 示例

展示如何使用大纲代码定义集合。

```csharp
var project = new Project(DataDir + "OutlineCodes.mpp");

Console.WriteLine("Count of outline code definitions: " + project.OutlineCodes.Count);
foreach (var outlineCode in project.OutlineCodes)
{
    Console.WriteLine("Field Name: " + outlineCode.FieldName);
    Console.WriteLine("Alias: " + outlineCode.Alias);
    Console.WriteLine();
}

// 添加自定义大纲代码定义。
var outlineCodeDefinition = new OutlineCodeDefinition { FieldId = ((int)ExtendedAttributeTask.OutlineCode3).ToString("D"), Alias = "My Outline Code" };

var outlineCodeDefinition2 = new OutlineCodeDefinition { FieldId = ((int)ExtendedAttributeTask.OutlineCode1).ToString("D"), Alias = "My Outline Code 2" };

if (!project.OutlineCodes.IsReadOnly)
{
    project.OutlineCodes.Add(outlineCodeDefinition);

    // 在位置插入大纲代码定义。
    project.OutlineCodes.Insert(0, outlineCodeDefinition2);
}

// 查找大纲代码定义的索引。
var index = project.OutlineCodes.IndexOf(outlineCodeDefinition);

// 编辑大纲代码定义
project.OutlineCodes[index].Alias = "New Alias";

// ...
// 使用大纲代码定义
// ...

// 删除大纲代码定义
if (project.OutlineCodes.Contains(outlineCodeDefinition))
{
    project.OutlineCodes.Remove(outlineCodeDefinition);
}

// 按索引删除大纲代码定义
project.OutlineCodes.RemoveAt(0);

var otherProject = new Project(DataDir + "Blank2010.mpp");

// 删除大纲代码定义
otherProject.OutlineCodes.Clear();

// 复制大纲代码定义
var outlineCodeDefinitions = new OutlineCodeDefinition[project.OutlineCodes.Count];
project.OutlineCodes.CopyTo(outlineCodeDefinitions, 0);

foreach (var definition in outlineCodeDefinitions)
{
    otherProject.OutlineCodes.Add(definition);
}

// ...
// 使用大纲代码定义
// ...

// 逐个删除大纲代码定义
List<OutlineCodeDefinition> definitions = otherProject.OutlineCodes.ToList();
foreach (var definition in definitions)
{
    otherProject.OutlineCodes.Remove(definition);
}
```

### 另见

* class [OutlineCodeDefinition](../outlinecodedefinition/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


