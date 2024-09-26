---
title: FilterCriteria.Operation
second_title: Aspose.Tasks for .NET API Reference
description: FilterCriteria property. Gets or sets the criterion established with FieldName Test and Value relates to other criteria in the filter
type: docs
weight: 40
url: /net/aspose.tasks/filtercriteria/operation/
---
## FilterCriteria.Operation property

Gets or sets the criterion established with FieldName, Test, and Value relates to other criteria in the filter.

```csharp
public FilterOperation Operation { get; set; }
```

## Examples

Shows how to read task filter criteria.

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

// print filter criteria as a string 
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

### See Also

* enum [FilterOperation](../../filteroperation/)
* class [FilterCriteria](../)
* namespace [Aspose.Tasks](../../filtercriteria/)
* assembly [Aspose.Tasks](../../../)


