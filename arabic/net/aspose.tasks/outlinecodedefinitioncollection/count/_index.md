---
title: "OutlineCodeDefinitionCollection.Count"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "OutlineCodeDefinitionCollection خاصية. يحصل على عدد العناصر الموجودة في هذه المجموعة"
type: docs
weight: 10
url: /ar/net/aspose.tasks/outlinecodedefinitioncollection/count/
---
## OutlineCodeDefinitionCollection.Count property

يحصل على عدد العناصر الموجودة في هذه المجموعة.

```csharp
public int Count { get; }
```

## الأمثلة

يوضح كيفية العمل مع مجموعات تعريف رموز المخطط.

```csharp
var project = new Project(DataDir + "OutlineCodes.mpp");

Console.WriteLine("Count of outline code definitions: " + project.OutlineCodes.Count);
foreach (var outlineCode in project.OutlineCodes)
{
    Console.WriteLine("Field Name: " + outlineCode.FieldName);
    Console.WriteLine("Alias: " + outlineCode.Alias);
    Console.WriteLine();
}

// إضافة تعريف مخصص لـ outline code
var outlineCodeDefinition = new OutlineCodeDefinition { FieldId = ((int)ExtendedAttributeTask.OutlineCode3).ToString("D"), Alias = "My Outline Code" };

var outlineCodeDefinition2 = new OutlineCodeDefinition { FieldId = ((int)ExtendedAttributeTask.OutlineCode1).ToString("D"), Alias = "My Outline Code 2" };

if (!project.OutlineCodes.IsReadOnly)
{
    project.OutlineCodes.Add(outlineCodeDefinition);

    // إدراج تعريف رمز المخطط في موضع
    project.OutlineCodes.Insert(0, outlineCodeDefinition2);
}

// العثور على فهرس تعريف رمز المخطط
var index = project.OutlineCodes.IndexOf(outlineCodeDefinition);

// تحرير تعريف رمز المخطط التفصيلي
project.OutlineCodes[index].Alias = "New Alias";

// ...
// العمل مع تعريفات رمز المخطط التفصيلي
// ...

// إزالة تعريف رمز المخطط التفصيلي
if (project.OutlineCodes.Contains(outlineCodeDefinition))
{
    project.OutlineCodes.Remove(outlineCodeDefinition);
}

// إزالة تعريف رمز المخطط التفصيلي حسب الفهرس
project.OutlineCodes.RemoveAt(0);

var otherProject = new Project(DataDir + "Blank2010.mpp");

// إزالة تعريفات رمز المخطط التفصيلي
otherProject.OutlineCodes.Clear();

// نسخ تعريفات رمز المخطط التفصيلي
var outlineCodeDefinitions = new OutlineCodeDefinition[project.OutlineCodes.Count];
project.OutlineCodes.CopyTo(outlineCodeDefinitions, 0);

foreach (var definition in outlineCodeDefinitions)
{
    otherProject.OutlineCodes.Add(definition);
}

// ...
// العمل مع تعريفات رمز المخطط التفصيلي
// ...

// إزالة تعريفات رمز المخطط التفصيلي واحدة تلو الأخرى
List<OutlineCodeDefinition> definitions = otherProject.OutlineCodes.ToList();
foreach (var definition in definitions)
{
    otherProject.OutlineCodes.Remove(definition);
}
```

### انظر أيضًا

* class [OutlineCodeDefinitionCollection](../)
* namespace [Aspose.Tasks](../../outlinecodedefinitioncollection/)
* assembly [Aspose.Tasks](../../../)


