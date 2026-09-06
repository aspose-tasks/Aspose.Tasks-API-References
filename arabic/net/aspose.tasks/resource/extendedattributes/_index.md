---
title: "Resource.ExtendedAttributes"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Resource. يحصل على قيم سمة موسعة"
type: docs
weight: 320
url: /ar/net/aspose.tasks/resource/extendedattributes/
---
## Resource.ExtendedAttributes property

يحصل على قيم سمة موسّعة.

```csharp
public ExtendedAttributeCollection ExtendedAttributes { get; }
```

## ملاحظات

هناك قطعتان من البيانات ضرورية - مؤشر يعود إلى جدول السمة الموسعة الذي يُحدَّد إما بالمعرّف الفريد أو معرف الحقل، والقيمة التي تُحدَّد إما بالقيمة نفسها أو بمؤشر يعود إلى قائمة القيم.

## الأمثلة

يعرض كيفية إضافة سمات الموارد الموسعة.

```csharp
var project = new Project(DataDir + "ResourceExtendedAttributes.mpp");

// تعريف سمة موسعة
var definition = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Number1);
if (definition == null)
{
    definition = ExtendedAttributeDefinition.CreateResourceDefinition(ExtendedAttributeResource.Number1, "Age");
    project.ExtendedAttributes.Add(definition);
}

// إنشاء سمة موسعة وتعيين قيمتها
var attribute = definition.CreateExtendedAttribute();
attribute.NumericValue = 30.5345m;

// إضافة مورد جديد وسمةه الموسعة   
var resource = project.Resources.Add("R1");
resource.ExtendedAttributes.Add(attribute);

project.Save(OutDir + "ResourceExtendedAttributes_out.mpp", SaveFileFormat.Mpp);
```

### انظر أيضًا

* class [ExtendedAttributeCollection](../../extendedattributecollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


