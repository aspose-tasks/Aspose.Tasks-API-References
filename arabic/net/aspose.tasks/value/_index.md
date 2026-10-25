---
title: "الفئة Value"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.Value. تمثّل قيمة في قائمة القيم"
type: docs
weight: 2800
url: /ar/net/aspose.tasks/value/
---
## Value class

يمثّل قيمة في قائمة القيم.

```csharp
public class Value
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [Value](value/)() | يُهيّئ مثيلاً جديداً من الفئة `Value`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [DateTimeValue](../../aspose.tasks/value/datetimevalue/) { get; set; } | يحصل أو يعيّن القيمة الفعلية إذا كان يمكن تمثيلها كـ DateTime. القيمة الافتراضية هي MinValue. |
| [Description](../../aspose.tasks/value/description/) { get; set; } | يحصل أو يعيّن وصف القيمة. |
| [Duration](../../aspose.tasks/value/duration/) { get; set; } | يحصل أو يعيّن القيمة الفعلية المستخدمة لتمثيل المدة. |
| [Id](../../aspose.tasks/value/id/) { get; set; } | يحصل أو يعيّن المعرف الفريد للقيمة عبر المشروع. |
| [NumericValue](../../aspose.tasks/value/numericvalue/) { get; set; } | يحصل أو يعيّن القيمة الفعلية المستخدمة لتمثيل الرقم أو قيمة التكلفة. |
| [Phonetic](../../aspose.tasks/value/phonetic/) { get; set; } | يحصل أو يعيّن المعلومات الصوتية حول اسم الحقل المخصص. |
| [StringValue](../../aspose.tasks/value/stringvalue/) { get; set; } | يحصل أو يعيّن القيمة الفعلية المستخدمة لتمثيل سلسلة النص. |
| [Val](../../aspose.tasks/value/val/) { get; set; } | يحصل أو يعيّن القيمة الفعلية في التمثيل الداخلي. يُفضَّل استخدام الخصائص ذات النوع القوي المذكورة أدناه. |
| [ValueGuid](../../aspose.tasks/value/valueguid/) { get; } | يحصل على GUID يحدد هذه القيمة بين القيم الأخرى في المشروع بأكمله. |

## الأمثلة

يعرض كيفية قراءة العمل باستخدام قيم البحث.

```csharp
var project = new Project(DataDir + "ReadTaskExtendedAttributes.mpp");

// إنشاء تعريف سمة موسعة من نوع النص
var textLookup = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Text,
    ExtendedAttributeTask.Text2,
    "Task Towns Name");

// إضافة قيم بحث لتعريف السمة الموسعة
textLookup.AddLookupValue(new Value { Id = 1, StringValue = "Town1", Description = "This is Town1", Phonetic = "Town One" });
textLookup.AddLookupValue(new Value { Id = 2, StringValue = "Town2", Description = "This is Town2", Phonetic = "Town Two" });

Console.WriteLine("Iterate over text lookup values:");
foreach (var value in textLookup.ValueList)
{
    Console.WriteLine("Id: " + value.Id);
    Console.WriteLine("GUID: " + value.ValueGuid);
    Console.WriteLine("Value: " + value.Val);
    Console.WriteLine("String Value: " + value.StringValue);
    Console.WriteLine("Description: " + value.Description);
    Console.WriteLine("Phonetic: " + value.Phonetic);
    Console.WriteLine();
}

// إنشاء تعريف سمة موسعة من نوع المدة
var durationLookup = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Duration,
    ExtendedAttributeTask.Duration1,
    "Custom Durations");

// إضافة قيم بحث لتعريف السمة الموسعة
durationLookup.AddLookupValue(new Value { Id = 3, Duration = project.GetDuration(4, TimeUnitType.Hour), Description = "4 hours", Phonetic = "Four hours" });
durationLookup.AddLookupValue(new Value { Id = 4, Duration = project.GetDuration(8, TimeUnitType.Hour), Description = "1 day", Phonetic = "One day" });
durationLookup.AddLookupValue(new Value { Id = 5, Duration = project.GetDuration(1, TimeUnitType.Hour), Description = "1 hour", Phonetic = "One hour" });
durationLookup.AddLookupValue(new Value { Id = 6, Duration = project.GetDuration(10, TimeUnitType.Day), Description = "10 days", Phonetic = "Ten days" });

Console.WriteLine("Iterate over duration lookup values:");
foreach (var value in durationLookup.ValueList)
{
    Console.WriteLine("Id: " + value.Id);
    Console.WriteLine("GUID: " + value.ValueGuid);
    Console.WriteLine("Value: " + value.Val);
    Console.WriteLine("Duration: " + value.Duration);
    Console.WriteLine("Description: " + value.Description);
    Console.WriteLine("Phonetic: " + value.Phonetic);
    Console.WriteLine();
}

// إنشاء تعريف سمة موسعة من نوع التاريخ
var dateLookup = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Date,
    ExtendedAttributeTask.Date1,
    "Custom Date");
dateLookup.AddLookupValue(new Value { Id = 7, DateTimeValue = new DateTime(2020, 4, 27, 8, 0, 0), Description = "Start Date", Phonetic = "Start Date" });

Console.WriteLine("Iterate over date lookup values:");
foreach (var value in dateLookup.ValueList)
{
    Console.WriteLine("Id: " + value.Id);
    Console.WriteLine("GUID: " + value.ValueGuid);
    Console.WriteLine("Value: " + value.Val);
    Console.WriteLine("DateTime Value: " + value.DateTimeValue);
    Console.WriteLine("Description: " + value.Description);
    Console.WriteLine("Phonetic: " + value.Phonetic);
    Console.WriteLine();
}

// إنشاء تعريف سمة موسعة من نوع الرقم
var numericLookup = ExtendedAttributeDefinition.CreateLookupTaskDefinition(
    CustomFieldType.Number,
    ExtendedAttributeTask.Number1,
    "Number of tons");
numericLookup.AddLookupValue(new Value { Id = 8, NumericValue = 10, Description = "10 tons", Phonetic = "Ten tons" });
numericLookup.AddLookupValue(new Value { Id = 9, NumericValue = 20, Description = "20 tons", Phonetic = "Twenty tons" });
numericLookup.AddLookupValue(new Value { Id = 10, NumericValue = 30, Description = "30 tons", Phonetic = "Thirty tons" });

Console.WriteLine("Iterate over numeric lookup values:");
foreach (var value in numericLookup.ValueList)
{
    Console.WriteLine("Id: " + value.Id);
    Console.WriteLine("GUID: " + value.ValueGuid);
    Console.WriteLine("Value: " + value.Val);
    Console.WriteLine("Numeric Value: " + value.NumericValue);
    Console.WriteLine("Description: " + value.Description);
    Console.WriteLine("Phonetic: " + value.Phonetic);
    Console.WriteLine();
}

project.ExtendedAttributes.Add(textLookup);
project.ExtendedAttributes.Add(durationLookup);
project.ExtendedAttributes.Add(dateLookup);
project.ExtendedAttributes.Add(numericLookup);
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


