---
title: "FilterCriteria.CriteriaRows"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية FilterCriteria. تحصل على قائمة صفوف FilterCriteria الفرعية. إذا كان الفلتر يحتوي على أكثر من صف معيار واحد، فإن تأثير عامل And هو أن المعايير لكلا الصفين يجب أن تتحقق لكي يتم عرض المهمة أو المورد نتيجة لهذا الفلتر. تأثير عامل Or هو أن المعايير لصف واحد أو الآخر يجب أن تتحقق."
type: docs
weight: 20
url: /ar/net/aspose.tasks/filtercriteria/criteriarows/
---
## FilterCriteria.CriteriaRows property

يحصل على قائمة صفوف [`FilterCriteria`](../) الفرعية. إذا كان الفلتر يحتوي على أكثر من صف معيار واحد، فإن تأثير عامل And هو أن المعايير لكلا الصفين يجب أن تتحقق لكي يتم عرض المهمة أو المورد نتيجة لهذا الفلتر. تأثير عامل Or هو أن المعايير لصف واحد أو الآخر يجب أن تتحقق.

```csharp
public List<FilterCriteria> CriteriaRows { get; }
```

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

* class [FilterCriteria](../)
* namespace [Aspose.Tasks](../../filtercriteria/)
* assembly [Aspose.Tasks](../../../)


