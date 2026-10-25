---
title: "Sınıf ResourceAssignmentCollection"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.ResourceAssignmentCollection sınıfı. ResourceAssignment nesnelerinin bir koleksiyonunu temsil eder"
type: docs
weight: 1760
url: /tr/net/aspose.tasks/resourceassignmentcollection/
---
## ResourceAssignmentCollection class

[`ResourceAssignment`](../resourceassignment/) nesnelerinin bir koleksiyonunu temsil eder.

```csharp
public class ResourceAssignmentCollection : IList<ResourceAssignment>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Count](../../aspose.tasks/resourceassignmentcollection/count/) { get; } | ResourceAssignmentCollection içinde bulunan nesne sayısını alır. |
| [IsReadOnly](../../aspose.tasks/resourceassignmentcollection/isreadonly/) { get; } | Bu koleksiyonun yalnızca okunabilir olup olmadığını gösteren bir değeri alır. |
| [Item](../../aspose.tasks/resourceassignmentcollection/item/) { get; set; } | Belirtilen indeksteki öğeyi döndürür. |
| [ParentProject](../../aspose.tasks/resourceassignmentcollection/parentproject/) { get; } | ResourceAssignmentCollection nesnesinin üst proje (parent project) bilgisini alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.tasks/resourceassignmentcollection/add/#add_3)(ResourceAssignment) | Bu, ICollection'ın Add metodunun sadece NotSupportedException fırlatan taslak uygulamasıdır |
| [Add](../../aspose.tasks/resourceassignmentcollection/add/#add)(Task, Resource) | ResourceAssignmentCollection'a yeni bir atama ekler. |
| [Add](../../aspose.tasks/resourceassignmentcollection/add/#add_2)(Task, Resource, decimal) | ResourceAssignmentCollection'a yeni bir atama ekler. |
| [Add](../../aspose.tasks/resourceassignmentcollection/add/#add_1)(Task, Resource, double) | ResourceAssignmentCollection'a yeni bir atama ekler. |
| [GetByUid](../../aspose.tasks/resourceassignmentcollection/getbyuid/)(int) | Belirtilen uid'ye sahip bir atamayı döndürür. |
| [GetEnumerator](../../aspose.tasks/resourceassignmentcollection/getenumerator/)() | Bu koleksiyon için bir enumerator döndürür. |
| [Remove](../../aspose.tasks/resourceassignmentcollection/remove/)(ResourceAssignment) | Belirtilen atamayı koleksiyondan kaldırır; koleksiyon yalnızca okunabilir değilse, aksi takdirde NotSupportedException fırlatır. |
| [RemoveAt](../../aspose.tasks/resourceassignmentcollection/removeat/)(int) | Belirtilen indeksteki atamayı koleksiyondan kaldırır; koleksiyon yalnızca okunabilir değilse, aksi takdirde NotSupportedException fırlatır. |
| [ToList](../../aspose.tasks/resourceassignmentcollection/tolist/)() | ResourceAssignmentCollection nesnesini [`ResourceAssignment`](../resourceassignment/) nesnelerinin bir listesine dönüştürür. |

## Örnekler

Kaynak atama koleksiyonlarıyla nasıl çalışılacağını gösterir.

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

// atanımla çalış...
Console.WriteLine("Is resource assignment collection read-only?: " + project.ResourceAssignments.IsReadOnly);

// koleksiyonu bir listeye dönüştür
List<ResourceAssignment> resourceAssignments = project.ResourceAssignments.ToList();

// liste üzerinde yinele
foreach (var ra in resourceAssignments)
{
    Console.WriteLine(ra.ToString());
}
```

### Ayrıca Bakınız

* class [ResourceAssignment](../resourceassignment/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


