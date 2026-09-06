---
title: "OutlineCodeDefinitionCollection.IsReadOnly"
second_title: "Aspose.Tasks for .NET API 参考"
description: "OutlineCodeDefinitionCollection 属性。获取一个值，指示此集合是否为只读，否则为 false。"
type: docs
weight: 20
url: /zh/net/aspose.tasks/outlinecodedefinitioncollection/isreadonly/
---
## OutlineCodeDefinitionCollection.IsReadOnly property

获取一个值，指示此集合是否为只读；否则为 false。

```csharp
public bool IsReadOnly { get; }
```

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

* class [OutlineCodeDefinitionCollection](../)
* namespace [Aspose.Tasks](../../outlinecodedefinitioncollection/)
* assembly [Aspose.Tasks](../../../)


