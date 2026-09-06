---
title: "OutlineCodeDefinitionCollection.Insert"
second_title: "Aspose.Tasks for .NET API 参考"
description: "OutlineCodeDefinitionCollection 方法。在指定索引处插入指定的项。"
type: docs
weight: 100
url: /zh/net/aspose.tasks/outlinecodedefinitioncollection/insert/
---
## OutlineCodeDefinitionCollection.Insert method

在指定索引处插入指定项。

```csharp
public void Insert(int index, OutlineCodeDefinition item)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| index | Int32 | 应在其插入项的指定零基索引。 |
| item | OutlineCodeDefinition | 要插入到此集合的指定项。 |

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

* class [OutlineCodeDefinition](../../outlinecodedefinition/)
* class [OutlineCodeDefinitionCollection](../)
* namespace [Aspose.Tasks](../../outlinecodedefinitioncollection/)
* assembly [Aspose.Tasks](../../../)


