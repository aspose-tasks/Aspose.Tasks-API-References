---
title: "فئة FilterCriteria"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "فئة Aspose.Tasks.FilterCriteria. تحدد المعايير التي يجب أن تلبيها المهام أو الموارد لتظهر في عرض MSP"
type: docs
weight: 630
url: /ar/net/aspose.tasks/filtercriteria/
---
## FilterCriteria class

يحدد المعايير التي يجب أن تفي بها المهام أو الموارد لتُعرض في عرض MSP.

```csharp
public class FilterCriteria
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [FilterCriteria](filtercriteria/)() | المنشئ الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [CriteriaRows](../../aspose.tasks/filtercriteria/criteriarows/) { get; } | يحصل على قائمة صفوف `FilterCriteria` الفرعية. إذا كان الفلتر يحتوي على أكثر من صف معيار واحد، فإن تأثير عامل And هو أن المعايير لكلا الصفين يجب أن تتحقق لكي يتم عرض المهمة أو المورد نتيجة لهذا الفلتر. تأثير عامل Or هو أن المعايير لأحد الصفين يجب أن تتحقق. |
| [Field](../../aspose.tasks/filtercriteria/field/) { get; set; } | يحصل أو يعيّن [`Field`](./field/) للتغيير. |
| [Operation](../../aspose.tasks/filtercriteria/operation/) { get; set; } | يحصل أو يعيّن المعيار المحدد بـ FieldName و Test و Value والذي يتعلق بمعايير أخرى في الفلتر. |
| [Test](../../aspose.tasks/filtercriteria/test/) { get; set; } | يحصل أو يعيّن نوع المقارنة بين FieldName و Value والذي يعمل كمعيار اختيار للفلتر. [`FilterComparisonType`](../filtercomparisontype/) |
| [Values](../../aspose.tasks/filtercriteria/values/) { get; } | يحصل على قيم الكائن للمقارنة مع قيمة الحقل المحدد بـ FieldName. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [IsFieldValue](../../aspose.tasks/filtercriteria/isfieldvalue/)() | يحصل على ما إذا كانت القيمة اليمنى لـ FilterCriteria إشارة إلى حقل، وليس قيمة ثابتة. |
| [SetValueField](../../aspose.tasks/filtercriteria/setvaluefield/)(Field) | يعيّن الحقل الذي ستُقارن قيمته مع قيمة الحقل المحدد بـ FieldName. |
| override [ToString](../../aspose.tasks/filtercriteria/tostring/)() | يرجع تمثيلًا نصيًا لنسخة فئة `FilterCriteria`. |

## الأمثلة

يوضح كيفية قراءة معايير فلتر المهمة.

```csharp
var project = new Project(DataDir + "Project2003.mpp");

var filter = project.TaskFilters.ToList()[1];
Console.WriteLine("Count of criteria rows: " + filter.Criteria.CriteriaRows.Count);
foreach (var row in filter.Criteria.CriteriaRows)
{
    Console.WriteLine("Field: " + row.Field);
    Console.WriteLine("Operation: " + row.Operation);
    Console.WriteLine("Test: " + row.Test);

    var values = row.Values.Where(c => c != null).ToArray();
    if (values.Length == 0)
    {
        continue;
    }

    Console.WriteLine("Value{0}: {1}", values.Length == 1 ? "" : "s", string.Join(", ", values));
}

// معايير فلتر الطباعة كنص.
Console.WriteLine(filter.Criteria.Operation.ToString());

var criteria1 = filter.Criteria.CriteriaRows[0];
Console.WriteLine("Criteria filter 1:");
Console.WriteLine(criteria1.ToString());

var criteria2 = filter.Criteria.CriteriaRows[1];
Console.WriteLine(criteria2.Operation.ToString());
Console.WriteLine(criteria2.CriteriaRows.Count);
Console.WriteLine("Criteria filter 2:");
Console.WriteLine(criteria2.ToString());

var criteria21 = criteria2.CriteriaRows[0];
Console.WriteLine("Criteria filter 21:");
Console.WriteLine(criteria21.ToString());

var criteria22 = criteria2.CriteriaRows[1];
Console.WriteLine("Criteria filter 22:");
Console.WriteLine(criteria22.ToString());
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


