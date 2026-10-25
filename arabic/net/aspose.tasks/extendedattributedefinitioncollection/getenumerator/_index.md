---
title: "ExtendedAttributeDefinitionCollection.GetEnumerator"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة ExtendedAttributeDefinitionCollection. تُرجع عدادًا لهذه المجموعة"
type: docs
weight: 100
url: /ar/net/aspose.tasks/extendedattributedefinitioncollection/getenumerator/
---
## ExtendedAttributeDefinitionCollection.GetEnumerator method

يرجع عدادًا لهذه المجموعة.

```csharp
public IEnumerator<ExtendedAttributeDefinition> GetEnumerator()
```

### قيمة الإرجاع

عداد لهذه المجموعة.

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

* class [ExtendedAttributeDefinition](../../extendedattributedefinition/)
* class [ExtendedAttributeDefinitionCollection](../)
* namespace [Aspose.Tasks](../../extendedattributedefinitioncollection/)
* assembly [Aspose.Tasks](../../../)


