---
title: "تعداد FilterComparisonType"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "تعداد Aspose.Tasks.FilterComparisonType. نوع المقارنة التي تتم بين FieldName و Value والتي تعمل كمعايير اختيار لمرشح أو مؤشر رسومي"
type: docs
weight: 620
url: /ar/net/aspose.tasks/filtercomparisontype/
---
## FilterComparisonType enumeration

نوع المقارنة التي تتم بين FieldName و Value والتي تعمل كمعيار اختيار لمرشح أو مؤشر رسومي.

```csharp
public enum FilterComparisonType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Equals | `6` | قيمة Field تساوي Value. |
| DoesNotEqual | `7` | قيمة Field لا تساوي Value. |
| IsGreaterThan | `2` | قيمة Field أكبر من Value. |
| IsGreaterThanOrEqualTo | `4` | قيمة Field أكبر من أو تساوي Value. |
| IsLessThan | `3` | قيمة Field أصغر من Value. |
| IsLessThanOrEqualTo | `5` | قيمة Field أصغر من أو تساوي Value. |
| IsWithin | `1` | قيمة Field ضمن Value. |
| IsNotWithin | `9` | قيمة Field ليست ضمن Value. |
| Contains | `8` | قيمة Field تحتوي على Value. |
| DoesNotContain | `10` | قيمة Field لا تحتوي على Value. |
| ContainsExactly | `11` | قيمة Field تحتوي على Value بالضبط. |
| IsOneOf | `12` | قيمة Field تساوي إحدى القيم المحددة. تُستخدم في AutoFilters. |
| Undefined | `0` | قيمة غير معرفة. |
| IsAnyValue | `255` | شرط 'Is any value'. ينطبق على المؤشرات الرسومية. |

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


