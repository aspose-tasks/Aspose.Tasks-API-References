---
title: "Project.ExtendedAttributes"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Project. تحصل على كائن ExtendedAttributeDefinitionCollection. مجموعة تعريفات الحقول المخصصة للسمات الموسعة المرتبطة بمشروع"
type: docs
weight: 410
url: /ar/net/aspose.tasks/project/extendedattributes/
---
## Project.ExtendedAttributes property

يحصل على كائن ExtendedAttributeDefinitionCollection. مجموعة تعريفات السمة الموسّعة (الحقول المخصّصة) المرتبطة بمشروع.

```csharp
public ExtendedAttributeDefinitionCollection ExtendedAttributes { get; }
```

## الأمثلة

يوضح كيفية العمل مع السمات الموسعة.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var definition = project.ExtendedAttributes.GetById((int)ExtendedAttributeTask.Text1);

// إذا لم يكن الحقل المخصص موجوداً في المشروع، قم بإنشائه.
if (definition == null)
{
    definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, "My text field");
    project.ExtendedAttributes.Add(definition);
}

// إنشاء سمة موسعة من التعريف
var attribute = definition.CreateExtendedAttribute();
attribute.TextValue = "Text attribute value";

// إضافة سمة موسعة إلى المهمة
var task = project.RootTask.Children.Add("Task 1");
task.ExtendedAttributes.Add(attribute);

project.Save(OutDir + "CreateExtendedAttributes_out.mpp", SaveFileFormat.Mpp);
```

### انظر أيضًا

* class [ExtendedAttributeDefinitionCollection](../../extendedattributedefinitioncollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


