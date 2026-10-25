---
title: "الفئة OutlineCodeDefinitionCollection"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.OutlineCodeDefinitionCollection. تمثل مجموعة من كائنات OutlineCodeDefinition."
type: docs
weight: 1180
url: /ar/net/aspose.tasks/outlinecodedefinitioncollection/
---
## OutlineCodeDefinitionCollection class

تمثل مجموعة من كائنات [`OutlineCodeDefinition`](../outlinecodedefinition/).

```csharp
public class OutlineCodeDefinitionCollection : IList<OutlineCodeDefinition>
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Count](../../aspose.tasks/outlinecodedefinitioncollection/count/) { get; } | يحصل على عدد العناصر الموجودة في هذه المجموعة. |
| [IsReadOnly](../../aspose.tasks/outlinecodedefinitioncollection/isreadonly/) { get; } | يحصل على قيمة تشير إلى ما إذا كانت هذه المجموعة للقراءة فقط؛ وإلا، false. |
| [Item](../../aspose.tasks/outlinecodedefinitioncollection/item/) { get; set; } | يرجع أو يعيّن العنصر في الفهرس المحدد. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Add](../../aspose.tasks/outlinecodedefinitioncollection/add/)(OutlineCodeDefinition) | يضيف العنصر المحدد إلى هذه المجموعة. |
| [Clear](../../aspose.tasks/outlinecodedefinitioncollection/clear/)() | يزيل جميع العناصر من هذه المجموعة. |
| [Contains](../../aspose.tasks/outlinecodedefinitioncollection/contains/)(OutlineCodeDefinition) | يرجع true إذا تم العثور على العنصر المحدد في هذه المجموعة؛ وإلا، false. |
| [CopyTo](../../aspose.tasks/outlinecodedefinitioncollection/copyto/)(OutlineCodeDefinition[], int) | ينسخ عناصر هذه المجموعة إلى المصفوفة المحددة، بدءًا من الفهرس المحدد للمصفوفة. |
| [GetEnumerator](../../aspose.tasks/outlinecodedefinitioncollection/getenumerator/)() | يرجع عدادًا لهذه المجموعة. |
| [IndexOf](../../aspose.tasks/outlinecodedefinitioncollection/indexof/)(OutlineCodeDefinition) | يحدد فهرس العنصر المحدد في هذه المجموعة. |
| [Insert](../../aspose.tasks/outlinecodedefinitioncollection/insert/)(int, OutlineCodeDefinition) | يدرج العنصر المحدد في الفهرس المحدد. |
| [Remove](../../aspose.tasks/outlinecodedefinitioncollection/remove/)(OutlineCodeDefinition) | يزيل الظهور الأول لكائن محدد من هذه المجموعة. |
| [RemoveAt](../../aspose.tasks/outlinecodedefinitioncollection/removeat/)(int) | يزيل عنصرًا في الفهرس المحدد. |
| [ToList](../../aspose.tasks/outlinecodedefinitioncollection/tolist/)() | يحول كائن OutlineCodeDefinitionCollection هذا إلى قائمة من كائنات [`OutlineCodeDefinition`](../outlinecodedefinition/). |

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

* class [OutlineCodeDefinition](../outlinecodedefinition/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


