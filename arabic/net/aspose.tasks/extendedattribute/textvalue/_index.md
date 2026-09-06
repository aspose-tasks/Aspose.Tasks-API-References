---
title: "ExtendedAttribute.TextValue"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية ExtendedAttribute. يحصل أو يضبط قيمة للسمات ذات النوع Text"
type: docs
weight: 80
url: /ar/net/aspose.tasks/extendedattribute/textvalue/
---
## ExtendedAttribute.TextValue property

يحصل أو يعيّن قيمة للسمات ذات النوع 'Text'.

```csharp
public string TextValue { get; set; }
```

### استثناءات

| استثناء | شرط |
| --- | --- |
| InvalidOperationException | يتم إلقاء الاستثناء إذا لم يتم تهيئة خاصية [`AttributeDefinition`](../attributedefinition/) أو إذا لم تكن السمة الحالية سمة نصية. |

## الأمثلة

يعرض كيفية إضافة سمات موسعة تستخدم صيغ تاريخ/وقت في MS Project.

```csharp
var project = new Project();
var task = project.RootTask.Children.Add("Task");

var numberDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Number1, null);
project.ExtendedAttributes.Add(numberDefinition);

var numberAttribute = numberDefinition.CreateExtendedAttribute();
task.ExtendedAttributes.Add(numberAttribute);

// اضبط صيغة ProjDateDiff واطبع قيمة السمة الموسعة.
numberDefinition.Formula = "ProjDateDiff(\"03/23/2015\",\"03/18/2015\")";
Console.WriteLine(numberAttribute.NumericValue);
numberDefinition.Formula = "ProjDateDiff(\"03/23/2015\",\"03/25/2015\")";
Console.WriteLine(numberAttribute.NumericValue);

var dateDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Date1, null);
project.ExtendedAttributes.Add(dateDefinition);
var dateAttribute = dateDefinition.CreateExtendedAttribute();
task.ExtendedAttributes.Add(dateAttribute);

var durationDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Duration4, "Custom duration field");
project.ExtendedAttributes.Add(durationDefinition);
var durationAttribute = durationDefinition.CreateExtendedAttribute();
task.ExtendedAttributes.Add(durationAttribute);

var textDefinition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text5, "Custom text field");
project.ExtendedAttributes.Add(textDefinition);
var textAttribute = textDefinition.CreateExtendedAttribute();
task.ExtendedAttributes.Add(textAttribute);

// اضبط صيغة ProjDateSub واطبع قيمة السمة الموسعة.
dateDefinition.Formula = "ProjDateSub(\"3/19/2015\", \"1d\")";
Console.WriteLine(dateAttribute.DateValue);

// يمكننا ضبط صيغة ProjDurConv للخاصية ذات القيمة الزمنية وكذلك للخاصية ذات القيمة النصية.
// اضبط صيغة ProjDurConv للخاصية الموسعة ذات القيمة الزمنية واطبع قيمتها.
durationDefinition.Formula = "ProjDurConv([Duration], pjHours)";
Console.WriteLine(durationAttribute.DurationValue);

// اضبط صيغة ProjDurConv للخاصية الموسعة ذات القيمة النصية واطبع قيمتها.
textDefinition.Formula = "ProjDurConv([Duration], pjWeeks)";
Console.WriteLine(textAttribute.TextValue);

// اضبط صيغة Second واطبع قيمة السمة الموسعة.
numberDefinition.Formula = "Second(\"4/21/2015 2:53:41 AM\")";
Console.WriteLine(numberAttribute.NumericValue);

// اضبط صيغة Weekday واطبع قيمة السمة الموسعة.
numberDefinition.Formula = "Weekday(\"24/3/2015\", 1)";
Console.WriteLine(numberAttribute.NumericValue);
numberDefinition.Formula = "Weekday(\"24/3/2015\", 2)";
Console.WriteLine(numberAttribute.NumericValue);
numberDefinition.Formula = "Weekday(\"24/3/2015\", 3)";
Console.WriteLine(numberAttribute.NumericValue);
```

### انظر أيضًا

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


