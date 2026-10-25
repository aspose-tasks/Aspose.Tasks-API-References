---
title: "Table.TableFields"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Table. تحصل على مجموعة TableFields التي تمثل الحقول في الجدول."
type: docs
weight: 90
url: /ar/net/aspose.tasks/table/tablefields/
---
## Table.TableFields property

يحصل على مجموعة TableFields التي تمثل الحقول في الجدول.

```csharp
public TableFieldCollection TableFields { get; }
```

## الأمثلة

يظهر كيفية التعامل مع جداول المشروع.

```csharp
var project = new Project(DataDir + "Project5.mpp");
var task = project.RootTask.Children.Add("New Activity");

// تعريف سمة مخصصة جديدة.
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, null);
project.ExtendedAttributes.Add(definition);

// أضف سمة نص مخصصة إلى المهمة التي تم إنشاؤها.
task.ExtendedAttributes.Add(definition.CreateExtendedAttribute("Activity attribute"));

// تخصيص الجدول عن طريق إضافة حقل سمة النص
var field = new TableField();
field.Field = Field.TaskText1;
field.Width = 20;
field.Title = "Custom attribute";
field.AlignTitle = HorizontalStringAlignment.Center;
field.AlignData = HorizontalStringAlignment.Center;

var table = project.Tables.ToList()[0];
table.TableFields.Insert(3, field);

project.Save(OutDir + "ConfigureGanttChart_out.mpp", new MPPSaveOptions { WriteViewData = true });
```

### انظر أيضًا

* class [TableFieldCollection](../../tablefieldcollection/)
* class [Table](../)
* namespace [Aspose.Tasks](../../table/)
* assembly [Aspose.Tasks](../../../)


