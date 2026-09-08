---
title: "FilterCriteria.CriteriaRows"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство FilterCriteria. Получает список дочерних строк FilterCriteria. Если фильтр содержит более одной строки критерия, то действие оператора И заключается в том, что критерии обеих строк должны быть выполнены, чтобы задача или ресурс отобразились в результате этого фильтра. Действие оператора ИЛИ заключается в том, что критерий одной из строк должен быть выполнен."
type: docs
weight: 20
url: /ru/net/aspose.tasks/filtercriteria/criteriarows/
---
## FilterCriteria.CriteriaRows property

Получает список дочерних строк [`FilterCriteria`](../). Если фильтр содержит более одной строки критерия, то действие оператора И заключается в том, что критерии обеих строк должны быть выполнены, чтобы задача или ресурс отобразились в результате этого фильтра. Действие оператора ИЛИ заключается в том, что критерий одной из строк должен быть выполнен.

```csharp
public List<FilterCriteria> CriteriaRows { get; }
```

## Примеры

Показывает, как читать критерии фильтра задач.

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

// Печать критериев фильтра в виде строки
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

### См. также

* class [FilterCriteria](../)
* namespace [Aspose.Tasks](../../filtercriteria/)
* assembly [Aspose.Tasks](../../../)


