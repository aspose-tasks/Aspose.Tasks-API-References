---
title: "Класс ResourceAssignmentCollection"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.ResourceAssignmentCollection. Представляет коллекцию объектов ResourceAssignment."
type: docs
weight: 1760
url: /ru/net/aspose.tasks/resourceassignmentcollection/
---
## ResourceAssignmentCollection class

Представляет коллекцию объектов [`ResourceAssignment`](../resourceassignment/).

```csharp
public class ResourceAssignmentCollection : IList<ResourceAssignment>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Count](../../aspose.tasks/resourceassignmentcollection/count/) { get; } | Получает количество объектов, содержащихся в ResourceAssignmentCollection. |
| [IsReadOnly](../../aspose.tasks/resourceassignmentcollection/isreadonly/) { get; } | Возвращает значение, указывающее, является ли эта коллекция только для чтения. |
| [Item](../../aspose.tasks/resourceassignmentcollection/item/) { get; set; } | Возвращает элемент по указанному индексу. |
| [ParentProject](../../aspose.tasks/resourceassignmentcollection/parentproject/) { get; } | Получает родительский проект объекта ResourceAssignmentCollection. |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.tasks/resourceassignmentcollection/add/#add_3)(ResourceAssignment) | Это заглушка реализации метода Add интерфейса ICollection, который только бросает NotSupportedException |
| [Add](../../aspose.tasks/resourceassignmentcollection/add/#add)(Task, Resource) | Добавляет новое назначение в ResourceAssignmentCollection. |
| [Add](../../aspose.tasks/resourceassignmentcollection/add/#add_2)(Task, Resource, decimal) | Добавляет новое назначение в ResourceAssignmentCollection. |
| [Add](../../aspose.tasks/resourceassignmentcollection/add/#add_1)(Task, Resource, double) | Добавляет новое назначение в ResourceAssignmentCollection. |
| [GetByUid](../../aspose.tasks/resourceassignmentcollection/getbyuid/)(int) | Возвращает назначение с указанным uid. |
| [GetEnumerator](../../aspose.tasks/resourceassignmentcollection/getenumerator/)() | Возвращает перечислитель для этой коллекции. |
| [Remove](../../aspose.tasks/resourceassignmentcollection/remove/)(ResourceAssignment) | Удаляет указанное назначение из коллекции, если она не только для чтения, иначе генерирует NotSupportedException. |
| [RemoveAt](../../aspose.tasks/resourceassignmentcollection/removeat/)(int) | Удаляет назначение по указанному индексу, если коллекция не только для чтения, иначе генерирует NotSupportedException. |
| [ToList](../../aspose.tasks/resourceassignmentcollection/tolist/)() | Преобразует объект ResourceAssignmentCollection в список объектов [`ResourceAssignment`](../resourceassignment/). |

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

* class [ResourceAssignment](../resourceassignment/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


