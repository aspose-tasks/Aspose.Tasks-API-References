---
title: Class Baseline
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.Baseline class. Represents baseline values of a resource
type: docs
weight: 110
url: /net/aspose.tasks/baseline/
---
## Baseline class

Represents baseline values of a resource.

```csharp
public class Baseline : IComparable<Baseline>, IEquatable<Baseline>
```

## Constructors

| Name | Description |
| --- | --- |
| [Baseline](baseline/)() | The default constructor. |

## Properties

| Name | Description |
| --- | --- |
| [BaselineNumber](../../aspose.tasks/baseline/baselinenumber/) { get; set; } | Gets or sets the unique number of a baseline data record. |
| [Bcwp](../../aspose.tasks/baseline/bcwp/) { get; set; } | Gets or sets the budgeted cost of a work performed by a resource for a project to-date. |
| [Bcws](../../aspose.tasks/baseline/bcws/) { get; set; } | Gets or sets the budget cost of a work scheduled for a resource. |
| [Cost](../../aspose.tasks/baseline/cost/) { get; set; } | Gets or sets the projected cost of a resource when the baseline is saved. |
| [Work](../../aspose.tasks/baseline/work/) { get; set; } | Gets or sets the work assigned to a resource when the baseline is saved. The amount of assigned work to a resource when the baseline was saved. |

## Methods

| Name | Description |
| --- | --- |
| [CompareTo](../../aspose.tasks/baseline/compareto/)(Baseline) | IComparable interface implementation. Compares this instance to the specified Baseline object. |
| [Equals](../../aspose.tasks/baseline/equals/#equals)(Baseline) | Returns a value indicating whether this instance is equal to a specified object. |
| override [Equals](../../aspose.tasks/baseline/equals/#equals_1)(object) | Returns a value indicating whether this instance is equal to a specified object. |
| override [GetHashCode](../../aspose.tasks/baseline/gethashcode/)() | Returns a hash code value for the baseline. |
| [operator ==](../../aspose.tasks/baseline/op_equality/) | Returns a value indicating whether this instance is equal to a specified object. |
| [operator &gt;](../../aspose.tasks/baseline/op_greaterthan/) | Returns a value indicating whether this instance is greater than a specified object. |
| [operator &gt;=](../../aspose.tasks/baseline/op_greaterthanorequal/) | Returns a value indicating whether this instance is greater than or equal to a specified object. |
| [operator !=](../../aspose.tasks/baseline/op_inequality/) | Returns a value indicating whether this instance is not equal to a specified object. |
| [operator &lt;](../../aspose.tasks/baseline/op_lessthan/) | Returns a value indicating whether this instance is less than a specified object. |
| [operator &lt;=](../../aspose.tasks/baseline/op_lessthanorequal/) | Returns a value indicating whether this instance is less than or equal to a specified object. |

## Examples

Shows how to work with baselines of assignments.

```csharp
var project = new Project(DataDir + "AssignmentBaseline2007.mpp");

// assignment baselines are set when one sets the baseline on whole project
project.SetBaseline(BaselineType.Baseline);

// read assignment baseline information
foreach (var assignment in project.ResourceAssignments)
{
    foreach (var baseline in assignment.Baselines)
    {
        Console.WriteLine("Baseline Start: " + baseline.Start);
        Console.WriteLine("Baseline Finish: " + baseline.Finish);
        Console.WriteLine("Baseline Number: " + baseline.BaselineNumber);
        Console.WriteLine("Bcwp: " + baseline.Bcwp);
        Console.WriteLine("Bcws: " + baseline.Bcws);
        Console.WriteLine("Cost: " + baseline.Cost);
        Console.WriteLine("Work: " + baseline.Work);
        if (baseline.TimephasedData != null)
        {
            foreach (var td in baseline.TimephasedData)
            {
                Console.WriteLine("TD Start: " + td.Start);
                Console.WriteLine("TD Finish: " + td.Finish);
                Console.WriteLine("TD Timephased Data Type: " + td.TimephasedDataType);
                Console.WriteLine();
            }
        }

        Console.WriteLine();
    }

    Console.WriteLine();
}

// check baseline equality
var assn1 = project.ResourceAssignments.GetByUid(5);
var assn2 = project.ResourceAssignments.GetByUid(7);

var assignmentBaseline1 = assn1.Baselines.ToList()[0];
var assignmentBaseline2 = assn2.Baselines.ToList()[0];

// baselines can be compared by using 'Equals' method overloads
Console.WriteLine("Are baselines equal: " + assignmentBaseline1.Equals(assignmentBaseline2));

// or by using overloaded arithmetic operation
Console.WriteLine("Is baseline 1 less than baseline 2: " + (assignmentBaseline1 < assignmentBaseline2));

// the baseline hashcode is based on baseline number
Console.WriteLine("Assignment baseline 1 hashcode: " + assignmentBaseline1.GetHashCode());
Console.WriteLine("Assignment baseline 2 hashcode: " + assignmentBaseline2.GetHashCode());
```

### See Also

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


