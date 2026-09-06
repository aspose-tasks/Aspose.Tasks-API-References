---
title: "الفئة OutlineValueCollection"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.OutlineValueCollection. تمثل مجموعة من كائنات OutlineValue"
type: docs
weight: 1220
url: /ar/net/aspose.tasks/outlinevaluecollection/
---
## OutlineValueCollection class

تمثل مجموعة من كائنات [`OutlineValue`](../outlinevalue/).

```csharp
public class OutlineValueCollection : IList<OutlineValue>
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Count](../../aspose.tasks/outlinevaluecollection/count/) { get; } | يحصل على عدد العناصر الموجودة في هذه المجموعة. |
| [IsReadOnly](../../aspose.tasks/outlinevaluecollection/isreadonly/) { get; } | يحصل على قيمة تشير إلى ما إذا كانت هذه المجموعة للقراءة فقط. |
| [Item](../../aspose.tasks/outlinevaluecollection/item/) { get; set; } | يرجع أو يعيّن العنصر في الفهرس المحدد. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Add](../../aspose.tasks/outlinevaluecollection/add/)(OutlineValue) | يضيف العنصر المحدد إلى هذه المجموعة. |
| [Clear](../../aspose.tasks/outlinevaluecollection/clear/)() | يزيل جميع العناصر من هذه المجموعة. |
| [Contains](../../aspose.tasks/outlinevaluecollection/contains/)(OutlineValue) | يرجع true إذا تم العثور على العنصر المحدد في هذه المجموعة؛ وإلا، false. |
| [CopyTo](../../aspose.tasks/outlinevaluecollection/copyto/)(OutlineValue[], int) | ينسخ عناصر هذه المجموعة إلى المصفوفة المحددة، بدءًا من الفهرس المحدد للمصفوفة. |
| [GetEnumerator](../../aspose.tasks/outlinevaluecollection/getenumerator/)() | يرجع عدادًا لهذه المجموعة. |
| [IndexOf](../../aspose.tasks/outlinevaluecollection/indexof/)(OutlineValue) | يحدد فهرس العنصر المحدد في هذه المجموعة. |
| [Insert](../../aspose.tasks/outlinevaluecollection/insert/)(int, OutlineValue) | يدرج العنصر المحدد في الفهرس المحدد. |
| [Remove](../../aspose.tasks/outlinevaluecollection/remove/)(OutlineValue) | يزيل الظهور الأول لكائن محدد من هذه المجموعة. |
| [RemoveAt](../../aspose.tasks/outlinevaluecollection/removeat/)(int) | يزيل عنصرًا في الفهرس المحدد. |

## الأمثلة

يظهر كيفية العمل مع مجموعات قيم المخطط.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

// مسح مجموعات القيم
foreach (var outlineCode in project.OutlineCodes)
{
    // مسح أقنعة المخطط
    if (outlineCode.Values.Count <= 0)
    {
        continue;
    }

    if (!outlineCode.Values.IsReadOnly)
    {
        outlineCode.Values.Clear();
    }
}

var codeDefinition = new OutlineCodeDefinition
                         {
                             Alias = "New task outline code1", FieldId = ((int)ExtendedAttributeTask.OutlineCode1).ToString(), FieldName = "Outline Code1"
                         };
var value = new OutlineValue { Description = "Value description", ValueId = 1, Value = "123456", Type = OutlineValueType.Number };
codeDefinition.Values.Add(value);
project.OutlineCodes.Add(codeDefinition);

// تحديث القيمة عبر الوصول إلى الفهرس
codeDefinition.Values[0].Value = "654321";

// التكرار على قيم المخطط
foreach (var definitionValue in codeDefinition.Values)
{
    Console.WriteLine("Value: " + definitionValue.Value);
    Console.WriteLine("Value Id: " + definitionValue.ValueId);
    Console.WriteLine("Value Guid: " + definitionValue.ValueGuid);
    Console.WriteLine();
}

// ...
// العمل مع قيم المخطط
// ...

// إزالة قيمة عند الحاجة
if (codeDefinition.Values.Contains(value))
{
    codeDefinition.Values.Remove(value);
}

// إدراج قيمة في الموضع الأول
codeDefinition.Values.Insert(0, value);

// التحقق من موضع القيمة المدخلة
Console.WriteLine("Index of inserted value: " + codeDefinition.Values.IndexOf(value));

// ...
// العمل مع قيم المخطط
// ...

// إزالة القيمة الأخيرة من المجموعة
codeDefinition.Values.RemoveAt(codeDefinition.Values.Count - 1);

// يمكن للمرء إنشاء تعريف شفرة مخطط آخر
var codeDefinition2 = new OutlineCodeDefinition
                          {
                              Alias = "New outline code 2", FieldId = ((int)ExtendedAttributeTask.OutlineCode2).ToString(), FieldName = "Outline Code2"
                          };

// ثم نسخ قيم المخطط
var outlineValues = new OutlineValue[codeDefinition.Values.Count];
codeDefinition.Values.CopyTo(outlineValues, 0);

foreach (var outlineValue in outlineValues)
{
    codeDefinition2.Values.Add(outlineValue);
}
```

### انظر أيضًا

* class [OutlineValue](../outlinevalue/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


