---
title: Enum FilterComparisonType
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.FilterComparisonType enum. The type of comparison made between FieldName and Value that acts as selection criteria for a filter or graphical indicator
type: docs
weight: 620
url: /net/aspose.tasks/filtercomparisontype/
---
## FilterComparisonType enumeration

The type of comparison made between FieldName and Value that acts as selection criteria for a filter or graphical indicator.

```csharp
public enum FilterComparisonType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Equals | `6` | The value of Field equals Value. |
| DoesNotEqual | `7` | The value of Field does not equal Value. |
| IsGreaterThan | `2` | The value of Field is greater than Value. |
| IsGreaterThanOrEqualTo | `4` | The value of Field is greater than or equal to Value. |
| IsLessThan | `3` | The value of Field is less than Value. |
| IsLessThanOrEqualTo | `5` | The value of Field is less than or equal to Value. |
| IsWithin | `1` | The value of Field is within Value. |
| IsNotWithin | `9` | The value of Field is not within Value. |
| Contains | `8` | The value of Field contains Value. |
| DoesNotContain | `10` | The value of Field does not contain Value. |
| ContainsExactly | `11` | The value of Field exactly contains Value. |
| IsOneOf | `12` | The value of Field equals to one of the specified Values. Used in AutoFilters. |
| Undefined | `0` | Undefined value. |
| IsAnyValue | `255` | 'Is any value' condition. Applicable to graphical indicators. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


