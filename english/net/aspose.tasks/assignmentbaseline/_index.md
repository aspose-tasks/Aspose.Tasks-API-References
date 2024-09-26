---
title: Class AssignmentBaseline
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.AssignmentBaseline class. Represents Baseline of a resource assignment
type: docs
weight: 50
url: /net/aspose.tasks/assignmentbaseline/
---
## AssignmentBaseline class

Represents Baseline of a resource assignment.

```csharp
public class AssignmentBaseline : Baseline, IComparable<AssignmentBaseline>, 
    IEquatable<AssignmentBaseline>
```

## Constructors

| Name | Description |
| --- | --- |
| [AssignmentBaseline](assignmentbaseline/)() | The default constructor. |

## Properties

| Name | Description |
| --- | --- |
| [BaselineNumber](../../aspose.tasks/baseline/baselinenumber/) { get; set; } | Gets or sets the unique number of a baseline data record. |
| [Bcwp](../../aspose.tasks/baseline/bcwp/) { get; set; } | Gets or sets the budgeted cost of a work performed by a resource for a project to-date. |
| [Bcws](../../aspose.tasks/baseline/bcws/) { get; set; } | Gets or sets the budget cost of a work scheduled for a resource. |
| [Cost](../../aspose.tasks/baseline/cost/) { get; set; } | Gets or sets the projected cost of a resource when the baseline is saved. |
| [Finish](../../aspose.tasks/assignmentbaseline/finish/) { get; set; } | Gets or sets the scheduled finish date of the resource assignment when the baseline was saved. The finish date of the resource assignment when this baseline was saved. |
| [Start](../../aspose.tasks/assignmentbaseline/start/) { get; set; } | Gets or sets the scheduled start date of the resource assignment when the baseline was saved. The start date of the resource assignment when this baseline was saved. |
| [TimephasedData](../../aspose.tasks/assignmentbaseline/timephaseddata/) { get; set; } | Gets or sets the [`TimephasedDataCollection`](../timephaseddatacollection/) instance for this object. The time phased data associated with the resource assignment baseline. returns [`TimephasedDataCollection`](../timephaseddatacollection/) instance for this object.The collection of Time phased data associated with this baseline. |
| [Work](../../aspose.tasks/baseline/work/) { get; set; } | Gets or sets the work assigned to a resource when the baseline is saved. The amount of assigned work to a resource when the baseline was saved. |

## Methods

| Name | Description |
| --- | --- |
| [CompareTo](../../aspose.tasks/assignmentbaseline/compareto/#compareto)(AssignmentBaseline) | IComparable interface implementation. Compares this instance to the specified Baseline object. |
| [CompareTo](../../aspose.tasks/baseline/compareto/)(Baseline) | IComparable interface implementation. Compares this instance to the specified Baseline object. |
| [Equals](../../aspose.tasks/assignmentbaseline/equals/#equals)(AssignmentBaseline) | Returns a value indicating whether this instance is equal to the specified AssignmentBaseline object. |
| [Equals](../../aspose.tasks/baseline/equals/)(Baseline) | Returns a value indicating whether this instance is equal to a specified object. |
| override [Equals](../../aspose.tasks/assignmentbaseline/equals/#equals_2)(object) | Returns a value indicating whether this instance is equal to a specified object. |
| override [GetHashCode](../../aspose.tasks/assignmentbaseline/gethashcode/)() |  |

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

* class [Baseline](../baseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


