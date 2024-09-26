---
title: Project.TaskFilters
second_title: Aspose.Tasks for .NET API Reference
description: Project property. Gets all the taskbased filter definitions. TaskFilters is a collection of Filter objects
type: docs
weight: 900
url: /net/aspose.tasks/project/taskfilters/
---
## Project.TaskFilters property

Gets all the task-based filter definitions. TaskFilters is a collection of [`Filter`](../../filter/) objects.

```csharp
public FilterCollection TaskFilters { get; }
```

## Examples

Shows how to read project task filters.

```csharp
var project = new Project(DataDir + "Project2003.mpp");

var filter = project.TaskFilters.ToList()[1];
Console.WriteLine(filter.Criteria.CriteriaRows.Count);
Console.WriteLine(filter.Criteria.Operation.ToString());

var criteria1 = filter.Criteria.CriteriaRows[0];
Console.WriteLine(criteria1.Test.ToString());
Console.WriteLine(criteria1.Field.ToString());
Console.WriteLine(criteria1.Values[0].ToString());

var criteria2 = filter.Criteria.CriteriaRows[1];
Console.WriteLine(criteria2.Operation.ToString());
Console.WriteLine(criteria2.CriteriaRows.Count);

var criteria21 = criteria2.CriteriaRows[0];
Console.WriteLine(criteria21.Test.ToString());
Console.WriteLine(criteria21.Field.ToString());
Console.WriteLine(criteria21.Values[0].ToString());

var criteria22 = criteria2.CriteriaRows[1];
Console.WriteLine(criteria22.Test.ToString());
Console.WriteLine(criteria22.Field.ToString());
Console.WriteLine(criteria22.Values[0].ToString());
Console.WriteLine(filter.Criteria);
```

### See Also

* class [FilterCollection](../../filtercollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


