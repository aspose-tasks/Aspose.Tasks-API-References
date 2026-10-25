---
title: "التعداد FilterOperation"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "التعداد Aspose.Tasks.FilterOperation. يحدد كيف يرتبط المعيار المُنشأ باستخدام FieldName و FilterComparisonType و Value بمعايير أخرى في الفلتر."
type: docs
weight: 640
url: /ar/net/aspose.tasks/filteroperation/
---
## FilterOperation enumeration

يحدد كيفية ارتباط المعيار الذي تم إنشاؤه باستخدام FieldName و FilterComparisonType و Value بالمعايير الأخرى في المرشح.

```csharp
public enum FilterOperation
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Undefined | `0` | غير معرف. |
| And | `1` | عامل AND. |
| Or | `2` | عامل OR. |

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


