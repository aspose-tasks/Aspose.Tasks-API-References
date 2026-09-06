---
title: "الفئة OutlineCodeCollection"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.OutlineCodeCollection. تمثل مجموعة من كائنات OutlineCode"
type: docs
weight: 1160
url: /ar/net/aspose.tasks/outlinecodecollection/
---
## OutlineCodeCollection class

تمثل مجموعة من كائنات [`OutlineCode`](../outlinecode/).

```csharp
public class OutlineCodeCollection : IList<OutlineCode>
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Count](../../aspose.tasks/outlinecodecollection/count/) { get; } | يحصل على عدد العناصر الموجودة في هذه المجموعة. |
| [IsReadOnly](../../aspose.tasks/outlinecodecollection/isreadonly/) { get; } | يحصل على قيمة تشير إلى ما إذا كانت هذه المجموعة للقراءة فقط؛ وإلا، false. |
| [Item](../../aspose.tasks/outlinecodecollection/item/) { get; set; } | يرجع أو يعيّن العنصر في الفهرس المحدد. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Add](../../aspose.tasks/outlinecodecollection/add/)(OutlineCode) | يضيف العنصر المحدد إلى هذه المجموعة. |
| [Clear](../../aspose.tasks/outlinecodecollection/clear/)() | يزيل جميع العناصر من هذه المجموعة. |
| [Contains](../../aspose.tasks/outlinecodecollection/contains/)(OutlineCode) | يرجع true إذا تم العثور على العنصر المحدد في هذه المجموعة؛ وإلا، false. |
| [CopyTo](../../aspose.tasks/outlinecodecollection/copyto/)(OutlineCode[], int) | ينسخ عناصر هذه المجموعة إلى المصفوفة المحددة، بدءًا من الفهرس المحدد للمصفوفة. |
| [GetEnumerator](../../aspose.tasks/outlinecodecollection/getenumerator/)() | يرجع عدادًا لهذه المجموعة. |
| [IndexOf](../../aspose.tasks/outlinecodecollection/indexof/)(OutlineCode) | يحدد فهرس العنصر المحدد في هذه المجموعة. |
| [Insert](../../aspose.tasks/outlinecodecollection/insert/)(int, OutlineCode) | يدرج العنصر المحدد في الفهرس المحدد. |
| [Remove](../../aspose.tasks/outlinecodecollection/remove/)(OutlineCode) | يزيل الظهور الأول لكائن محدد من هذه المجموعة. |
| [RemoveAt](../../aspose.tasks/outlinecodecollection/removeat/)(int) | يزيل عنصرًا في الفهرس المحدد. |

## الأمثلة

يعرض كيفية العمل مع مجموعات outline code.

```csharp
var project = new Project(DataDir + "OutlineCodes2003.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

for (var i = 0; i < collector.Tasks.Count; i++)
{
    var current = collector.Tasks[i];
    if (current.Get(Tsk.Id) == 0)
    {
        continue;
    }

    Console.WriteLine("Print outline codes for the " + current.Get(Tsk.Name) + " task.");
    Console.WriteLine("Count of outline codes: " + current.OutlineCodes.Count);
    foreach (var outlineCode in current.OutlineCodes)
    {
        Console.WriteLine("Field Id: " + outlineCode.FieldId);
        Console.WriteLine("Value Id: " + outlineCode.ValueId);
        Console.WriteLine("Value Guid: " + outlineCode.ValueGuid);
        Console.WriteLine();
    }
}

// إضافة تعريف مخصص لـ outline code
var outlineCodeDefinition = new OutlineCodeDefinition { FieldId = ((int)ExtendedAttributeTask.OutlineCode3).ToString("D"), Alias = "My Outline Code" };
project.OutlineCodes.Add(outlineCodeDefinition);

// إنشاء outline code
var value = new OutlineValue { Type = OutlineValueType.Text, Value = "Val1", Description = "Descr1", ValueId = 1 };
outlineCodeDefinition.Values.Add(value);

var codeOne = new OutlineCode { FieldId = outlineCodeDefinition.FieldId, ValueId = 1, ValueGuid = value.ValueGuid.ToString("D").ToUpperInvariant() };

var task = project.RootTask.Children.GetByUid(2);

// يمكن التحقق من أن المجموعة ليست للقراءة فقط
if (!task.OutlineCodes.IsReadOnly)
{
    task.OutlineCodes.Add(codeOne);
}

var codeZero = new OutlineCode { FieldId = outlineCodeDefinition.FieldId, ValueId = 0, ValueGuid = value.ValueGuid.ToString("D").ToUpperInvariant() };

task.OutlineCodes.Insert(0, codeZero);

var code2 = new OutlineCode { FieldId = outlineCodeDefinition.FieldId, ValueId = 2, ValueGuid = value.ValueGuid.ToString("D").ToUpperInvariant() };

// إدراج الكود مع 2 في موضع خاطئ
task.OutlineCodes.Insert(0, code2);

// إصلاح ذلك
var indexOf = task.OutlineCodes.IndexOf(code2);
task.OutlineCodes.RemoveAt(indexOf);

// إدراج الكود مع 2 في الموضع الصحيح
task.OutlineCodes.Insert(2, code2);

// تحقق من أن الكود تم إدراجه
Console.WriteLine("Is outline codes contains the inserted value: " + task.OutlineCodes.Contains(code2));

// ...
// العمل مع outline codes
// ...
var otherProject = new Project(DataDir + "OutlineCodes2003.mpp");
var otherTask = otherProject.RootTask.Children.GetById(2);

// إضافة تعريف مخصص لـ outline code
outlineCodeDefinition = new OutlineCodeDefinition { FieldId = ((int)ExtendedAttributeTask.OutlineCode3).ToString("D"), Alias = "My Outline Code" };
otherProject.OutlineCodes.Add(outlineCodeDefinition);

// إنشاء outline code
var otherValue = new OutlineValue { Type = OutlineValueType.Text, Value = "Val1", Description = "Descr1", ValueId = 1 };
outlineCodeDefinition.Values.Add(otherValue);

var outlineCodes = new OutlineCode[task.OutlineCodes.Count];
task.OutlineCodes.CopyTo(outlineCodes, 0);

foreach (var code in outlineCodes)
{
    otherTask.OutlineCodes.Add(code);
}

// ...
// العمل مع outline codes
// ...

// إزالة outline code
otherTask.OutlineCodes.RemoveAt(0);

while (otherTask.OutlineCodes.Count > 0)
{
    otherTask.OutlineCodes.Remove(otherTask.OutlineCodes[0]);
}

// مسح جميع القيم مرة واحدة
task.OutlineCodes.Clear();
```

### انظر أيضًا

* class [OutlineCode](../outlinecode/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


