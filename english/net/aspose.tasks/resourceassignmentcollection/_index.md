---
title: Class ResourceAssignmentCollection
second_title: Aspose.Tasks for .NET API Reference
description: Aspose.Tasks.ResourceAssignmentCollection class. Represents a collection of ResourceAssignment objects
type: docs
weight: 1730
url: /net/aspose.tasks/resourceassignmentcollection/
---
## ResourceAssignmentCollection class

Represents a collection of [`ResourceAssignment`](../resourceassignment/) objects.

```csharp
public class ResourceAssignmentCollection : IList<ResourceAssignment>
```

## Properties

| Name | Description |
| --- | --- |
| [Count](../../aspose.tasks/resourceassignmentcollection/count/) { get; } | Gets the number of objects contained in the ResourceAssignmentCollection. |
| [IsReadOnly](../../aspose.tasks/resourceassignmentcollection/isreadonly/) { get; } | Gets a value indicating whether this collection is read only. |
| [Item](../../aspose.tasks/resourceassignmentcollection/item/) { get; set; } | Returns the element at the specified index. |
| [ParentProject](../../aspose.tasks/resourceassignmentcollection/parentproject/) { get; } | Gets the parent project of the ResourceAssignmentCollection object. |

## Methods

| Name | Description |
| --- | --- |
| [Add](../../aspose.tasks/resourceassignmentcollection/add/#add_3)(ResourceAssignment) | This is the stub implementation of ICollection's Add method, that only throws NotSupportedException |
| [Add](../../aspose.tasks/resourceassignmentcollection/add/#add)(Task, Resource) | Adds new assignment to the ResourceAssignmentCollection. |
| [Add](../../aspose.tasks/resourceassignmentcollection/add/#add_2)(Task, Resource, decimal) | Adds new assignment to the ResourceAssignmentCollection. |
| [Add](../../aspose.tasks/resourceassignmentcollection/add/#add_1)(Task, Resource, double) | Adds new assignment to the ResourceAssignmentCollection. |
| [GetByUid](../../aspose.tasks/resourceassignmentcollection/getbyuid/)(int) | Returns an assignment with the specified uid. |
| [GetEnumerator](../../aspose.tasks/resourceassignmentcollection/getenumerator/)() | Returns an enumerator for this collection. |
| [Remove](../../aspose.tasks/resourceassignmentcollection/remove/)(ResourceAssignment) | Removes specified assignment from collection, if it is not read-only, otherwise throws NotSupportedException. |
| [RemoveAt](../../aspose.tasks/resourceassignmentcollection/removeat/)(int) | Removes assignment at specified index, if collection is not read-only, otherwise throws NotSupportedException. |
| [ToList](../../aspose.tasks/resourceassignmentcollection/tolist/)() | Converts the ResourceAssignmentCollection object to a list of [`ResourceAssignment`](../resourceassignment/) objects. |

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

* class [ResourceAssignment](../resourceassignment/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


