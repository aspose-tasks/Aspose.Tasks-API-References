---
title: "فئة OutlineCode"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "فئة Aspose.Tasks.OutlineCode. تمثل قيمة لكود المخطط التفصيلي"
type: docs
weight: 1150
url: /ar/net/aspose.tasks/outlinecode/
---
## OutlineCode class

يمثل قيمة لرمز المخطط التفصيلي.

```csharp
public class OutlineCode
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [OutlineCode](outlinecode/#constructor)() | ينشئ مثيلاً جديداً للفئة `OutlineCode`. |
| [OutlineCode](outlinecode/#constructor_1)(OutlineCodeDefinition, OutlineValue) | ينشئ مثيلاً جديداً للفئة `OutlineCode` باستخدام كود المخطط المحدد وإحدى قيمه. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [FieldId](../../aspose.tasks/outlinecode/fieldid/) { get; set; } | يحصل أو يعيّن القيمة العددية لحقل Id المخصص للمشروع. |
| [ValueGuid](../../aspose.tasks/outlinecode/valueguid/) { get; set; } | يحصل أو يعيّن GUID للقيمة في قائمة القيم. يتطابق ValueGuid مع FieldGuid في قائمة القيم. |
| [ValueId](../../aspose.tasks/outlinecode/valueid/) { get; set; } | يحصل أو يعيّن Id في قائمة القيم المرتبط بالتعريف في مجموعة كود المخطط. |

## ملاحظات

هناك عنصران من البيانات ضروريان - مؤشر إلى جدول كود المخطط المحدد بواسطة FieldId، والقيمة المحددة إما بواسطة ValueId أو مؤشر ValueGuid إلى قائمة القيم.

## الأمثلة

يوضح كيفية قراءة أكواد المخطط التفصيلي للمهمة.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

// قراءة أكواد المخطط التفصيلي
foreach (var task in project.RootTask.SelectAllChildTasks())
{
    if (task.OutlineCodes.Count <= 0)
    {
        continue;
    }

    Console.WriteLine("Print outline codes of the task: " + task.Get(Tsk.Name));
    foreach (var value in task.OutlineCodes)
    {
        Console.WriteLine("  Field Id: " + value.FieldId);
        Console.WriteLine("  Value Guid: " + value.ValueGuid);
        Console.WriteLine("  Value Id: " + value.ValueId);
    }
}
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


