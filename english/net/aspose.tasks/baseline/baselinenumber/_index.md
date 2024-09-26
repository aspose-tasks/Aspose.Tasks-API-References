---
title: Baseline.BaselineNumber
second_title: Aspose.Tasks for .NET API Reference
description: Baseline property. Gets or sets the unique number of a baseline data record
type: docs
weight: 20
url: /net/aspose.tasks/baseline/baselinenumber/
---
## Baseline.BaselineNumber property

Gets or sets the unique number of a baseline data record.

```csharp
public BaselineType BaselineNumber { get; set; }
```

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

* enum [BaselineType](../../baselinetype/)
* class [Baseline](../)
* namespace [Aspose.Tasks](../../baseline/)
* assembly [Aspose.Tasks](../../../)


