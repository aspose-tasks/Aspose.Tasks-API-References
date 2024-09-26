---
title: ResourceAssignmentCollection.Count
second_title: Aspose.Tasks for .NET API Reference
description: ResourceAssignmentCollection property. Gets the number of objects contained in the ResourceAssignmentCollection
type: docs
weight: 10
url: /net/aspose.tasks/resourceassignmentcollection/count/
---
## ResourceAssignmentCollection.Count property

Gets the number of objects contained in the ResourceAssignmentCollection.

```csharp
public int Count { get; }
```

## Examples

Shows how to work with resource assignment collections.

```csharp
var project = new Project(DataDir + "TemplateResource2010.mpp");

var task = project.RootTask.Children.Add("Task 1");
var resource = project.Resources.Add("Resource 1");
var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Start, new DateTime(2019, 9, 23, 9, 0, 0));
assignment.Set(Asn.Work, project.GetWork(40));
assignment.Set(Asn.Finish, new DateTime(2019, 9, 27, 18, 0, 0));

var assignmentWithUnits = project.ResourceAssignments.Add(task, resource, 1d);
assignmentWithUnits.Set(Asn.Start, new DateTime(2019, 9, 23, 9, 0, 0));
assignmentWithUnits.Set(Asn.Work, project.GetWork(40));
assignmentWithUnits.Set(Asn.Finish, new DateTime(2019, 9, 27, 18, 0, 0));

var assignmentWithCost = project.ResourceAssignments.Add(task, resource);
assignmentWithCost.Set(Asn.Start, new DateTime(2019, 9, 23, 9, 0, 0));
assignmentWithCost.Set(Asn.Work, project.GetWork(40));
assignmentWithCost.Set(Asn.Finish, new DateTime(2019, 9, 27, 18, 0, 0));

Console.WriteLine("Print assignments for the project: " + project.ResourceAssignments.ParentProject.Get(Prj.Name));
Console.WriteLine("Resource assignment count: " + project.ResourceAssignments.Count);
foreach (var resourceAssignment in project.ResourceAssignments)
{
    Console.WriteLine("Task Name: " + resourceAssignment.Get(Asn.Task).Get(Tsk.Name));
    Console.WriteLine("Uid: " + resourceAssignment.Get(Asn.Uid));
    Console.WriteLine("Start: " + resourceAssignment.Get(Asn.Start));
    Console.WriteLine("Work: " + resourceAssignment.Get(Asn.Work));
    Console.WriteLine("Finish: " + resourceAssignment.Get(Asn.Finish));
}

var assignmentByUid = project.ResourceAssignments.GetByUid(2);
Console.WriteLine("Assignment By Uid Start: " + assignmentByUid.Get(Asn.Start));

// work with assignment...
Console.WriteLine("Is resource assignment collection read-only?: " + project.ResourceAssignments.IsReadOnly);

// convert the collection into a list
List<ResourceAssignment> resourceAssignments = project.ResourceAssignments.ToList();

// iterate over the list
foreach (var ra in resourceAssignments)
{
    Console.WriteLine(ra.ToString());
}
```

### See Also

* class [ResourceAssignmentCollection](../)
* namespace [Aspose.Tasks](../../resourceassignmentcollection/)
* assembly [Aspose.Tasks](../../../)


