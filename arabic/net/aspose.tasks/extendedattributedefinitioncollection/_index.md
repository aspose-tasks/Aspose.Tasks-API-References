---
title: "الفئة ExtendedAttributeDefinitionCollection"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.ExtendedAttributeDefinitionCollection. تمثل مجموعة من كائنات ExtendedAttributeDefinition"
type: docs
weight: 550
url: /ar/net/aspose.tasks/extendedattributedefinitioncollection/
---
## ExtendedAttributeDefinitionCollection class

تمثل مجموعة من كائنات [`ExtendedAttributeDefinition`](../extendedattributedefinition/).

```csharp
public class ExtendedAttributeDefinitionCollection : IList<ExtendedAttributeDefinition>
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Count](../../aspose.tasks/extendedattributedefinitioncollection/count/) { get; } | يحصل على عدد العناصر الموجودة في هذه المجموعة. |
| [IsReadOnly](../../aspose.tasks/extendedattributedefinitioncollection/isreadonly/) { get; } | يحصل على قيمة تشير إلى ما إذا كانت هذه المجموعة للقراءة فقط. |
| [Item](../../aspose.tasks/extendedattributedefinitioncollection/item/) { get; set; } | يرجع أو يعيّن العنصر في الفهرس المحدد. |
| [ParentProject](../../aspose.tasks/extendedattributedefinitioncollection/parentproject/) { get; } | يحصل على مشروع أب للنسخة `ExtendedAttributeDefinitionCollection`. يرجع مشروعًا أبًا لهذه المجموعة. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Add](../../aspose.tasks/extendedattributedefinitioncollection/add/)(ExtendedAttributeDefinition) | يضيف العنصر المحدد إلى هذه المجموعة. |
| [Clear](../../aspose.tasks/extendedattributedefinitioncollection/clear/)() | يزيل جميع العناصر من هذه المجموعة. |
| [Contains](../../aspose.tasks/extendedattributedefinitioncollection/contains/)(ExtendedAttributeDefinition) | يرجع true إذا تم العثور على العنصر المحدد في هذه المجموعة؛ وإلا، false. |
| [CopyTo](../../aspose.tasks/extendedattributedefinitioncollection/copyto/)(ExtendedAttributeDefinition[], int) | ينسخ عناصر هذه المجموعة إلى المصفوفة المحددة، بدءًا من الفهرس المحدد للمصفوفة. |
| [GetById](../../aspose.tasks/extendedattributedefinitioncollection/getbyid/)(int) | يرجع تعريف سمة موسعة حسب المعرف |
| [GetEnumerator](../../aspose.tasks/extendedattributedefinitioncollection/getenumerator/)() | يرجع عدادًا لهذه المجموعة. |
| [IndexOf](../../aspose.tasks/extendedattributedefinitioncollection/indexof/)(ExtendedAttributeDefinition) | يحدد فهرس العنصر المحدد في هذه المجموعة. |
| [Insert](../../aspose.tasks/extendedattributedefinitioncollection/insert/)(int, ExtendedAttributeDefinition) | يدرج العنصر المحدد في الفهرس المحدد. |
| [Remove](../../aspose.tasks/extendedattributedefinitioncollection/remove/)(ExtendedAttributeDefinition) | يزيل الظهور الأول لكائن محدد من هذه المجموعة. |
| [RemoveAt](../../aspose.tasks/extendedattributedefinitioncollection/removeat/)(int) | يزيل عنصرًا في الفهرس المحدد. |
| [ToList](../../aspose.tasks/extendedattributedefinitioncollection/tolist/)() | يحول كائن ExtendedAttributeDefinitionCollection هذا إلى قائمة تحتوي على نسخ من الفئة [`ExtendedAttributeDefinition`](../extendedattributedefinition/). |

## الأمثلة

يوضح كيفية استخدام مجموعات تعريف السمة الموسعة.

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

if (!project.ExtendedAttributes.IsReadOnly)
{
    if (project.ExtendedAttributes.Count > 0)
    {
        // مسح تعريفات السمات الموسعة
        project.ExtendedAttributes.Clear();
    }
}

// إنشاء تعريف سمة موسعة لمهمة
var taskDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Start, ExtendedAttributeTask.Start7, "Start 7");
project.ExtendedAttributes.Add(taskDefinition);

Console.WriteLine("Iterate over extended attributes of " + project.ExtendedAttributes.ParentProject.Get(Prj.Name) + " project: ");
foreach (var attribute in project.ExtendedAttributes)
{
    Console.WriteLine("Attribute Alias: " + attribute.Alias);
    Console.WriteLine("Attribute CfType: " + attribute.CfType);
    Console.WriteLine();
}

Console.WriteLine();

// العمل مع تعريفات السمات الموسعة...
var resourceDefinition = ExtendedAttributeDefinition.CreateResourceDefinition(CustomFieldType.Cost, ExtendedAttributeResource.Cost5, "My cost");

if (!project.ExtendedAttributes.Contains(resourceDefinition))
{
    project.ExtendedAttributes.Add(resourceDefinition);
}

// العمل مع تعريفات السمات الموسعة...
var resourceDefinition2 = ExtendedAttributeDefinition.CreateResourceDefinition(CustomFieldType.Number, ExtendedAttributeResource.Cost1, "My Cost 2");

if (project.ExtendedAttributes.IndexOf(resourceDefinition2) < 0)
{
    project.ExtendedAttributes.Insert(0, resourceDefinition2);
}

// العمل مع تعريفات السمات الموسعة...

// إزالة سمة موسعة حسب الفهرس
project.ExtendedAttributes.RemoveAt(0);

Console.WriteLine("Print project's extended attributes: ");
Console.WriteLine("Count of project's extended attribute definitions: " + project.ExtendedAttributes.Count);

// استخدام وصول الفهرس للمجموعة
Console.WriteLine("Attribute 1 Alias: " + project.ExtendedAttributes[0].Alias);
Console.WriteLine("Attribute 1 CfType: " + project.ExtendedAttributes[0].CfType);
Console.WriteLine("Attribute 2 Alias: " + project.ExtendedAttributes[1].Alias);
Console.WriteLine("Attribute 2 CfType: " + project.ExtendedAttributes[1].CfType);

var otherProject = new Project();

// نسخ السمات إلى مشروع آخر
var attributes = new ExtendedAttributeDefinition[project.ExtendedAttributes.Count];
project.ExtendedAttributes.CopyTo(attributes, 0);

foreach (var attribute in attributes)
{
    otherProject.ExtendedAttributes.Add(attribute);
}

Console.WriteLine();
Console.WriteLine("Iterate over other project's extended attributes: ");
foreach (var attribute in otherProject.ExtendedAttributes)
{
    Console.WriteLine("Attribute Alias: " + attribute.Alias);
    Console.WriteLine("Attribute CfType: " + attribute.CfType);
    Console.WriteLine();
}

// إزالة جميع تعريفات السمات الموسعة
List<ExtendedAttributeDefinition> definitions = project.ExtendedAttributes.ToList();
foreach (var definition in definitions)
{
    project.ExtendedAttributes.Remove(definition);
}
```

### انظر أيضًا

* class [ExtendedAttributeDefinition](../extendedattributedefinition/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


