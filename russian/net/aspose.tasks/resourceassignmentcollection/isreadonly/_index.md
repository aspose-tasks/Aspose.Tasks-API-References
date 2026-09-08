---
title: "ResourceAssignmentCollection.IsReadOnly"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство ResourceAssignmentCollection. Возвращает значение, указывающее, является ли эта коллекция только для чтения"
type: docs
weight: 20
url: /ru/net/aspose.tasks/resourceassignmentcollection/isreadonly/
---
## ResourceAssignmentCollection.IsReadOnly property

Возвращает значение, указывающее, является ли эта коллекция только для чтения.

```csharp
public bool IsReadOnly { get; }
```

## Примеры

Показывает, как работать с коллекциями назначений ресурсов.

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

// работа с назначением...
Console.WriteLine("Is resource assignment collection read-only?: " + project.ResourceAssignments.IsReadOnly);

// преобразовать коллекцию в список
List<ResourceAssignment> resourceAssignments = project.ResourceAssignments.ToList();

// перебрать список
foreach (var ra in resourceAssignments)
{
    Console.WriteLine(ra.ToString());
}
```

### См. также

* class [ResourceAssignmentCollection](../)
* namespace [Aspose.Tasks](../../resourceassignmentcollection/)
* assembly [Aspose.Tasks](../../../)


