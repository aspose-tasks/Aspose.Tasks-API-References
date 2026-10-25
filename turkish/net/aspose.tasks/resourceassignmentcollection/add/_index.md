---
title: "ResourceAssignmentCollection.Add"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "ResourceAssignmentCollection yöntemi. ResourceAssignmentCollection'a yeni bir atama ekler"
type: docs
weight: 50
url: /tr/net/aspose.tasks/resourceassignmentcollection/add/
---
## Add(Task, Resource, double) {#add_1}

ResourceAssignmentCollection'a yeni bir atama ekler.

```csharp
public ResourceAssignment Add(Task task, Resource resource, double units)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| görev | Görev | Atanacak bir görev. |
| kaynak | Kaynak | Atanacak bir kaynak. |
| birimler | Double | Yeni bir atama için birim sayısı. |

### Dönüş Değeri

Atama eklendi.

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

* class [ResourceAssignment](../../resourceassignment/)
* class [Task](../../task/)
* class [Resource](../../resource/)
* class [ResourceAssignmentCollection](../)
* namespace [Aspose.Tasks](../../resourceassignmentcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(Task, Resource, decimal) {#add_2}

ResourceAssignmentCollection'a yeni bir atama ekler.

```csharp
public ResourceAssignment Add(Task task, Resource resource, decimal cost)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| görev | Görev | Atanacak bir görev. |
| kaynak | Kaynak | Atanacak bir maliyet kaynağı. |
| maliyet | Decimal | Yeni bir atama için maliyet. |

### Dönüş Değeri

Atama eklendi.

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

* class [ResourceAssignment](../../resourceassignment/)
* class [Task](../../task/)
* class [Resource](../../resource/)
* class [ResourceAssignmentCollection](../)
* namespace [Aspose.Tasks](../../resourceassignmentcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(Task, Resource) {#add}

ResourceAssignmentCollection'a yeni bir atama ekler.

```csharp
public ResourceAssignment Add(Task task, Resource resource)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| görev | Görev | Atanacak bir görev. |
| kaynak | Kaynak | Atanacak bir kaynak. |

### Dönüş Değeri

Atama eklendi.

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

* class [ResourceAssignment](../../resourceassignment/)
* class [Task](../../task/)
* class [Resource](../../resource/)
* class [ResourceAssignmentCollection](../)
* namespace [Aspose.Tasks](../../resourceassignmentcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(ResourceAssignment) {#add_3}

Bu, ICollection'ın Add metodunun sadece NotSupportedException fırlatan taslak uygulamasıdır

```csharp
public void Add(ResourceAssignment item)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| öğe | ResourceAssignment | Kaldırılacak öğe. |

### Ayrıca Bakınız

* class [ResourceAssignment](../../resourceassignment/)
* class [ResourceAssignmentCollection](../)
* namespace [Aspose.Tasks](../../resourceassignmentcollection/)
* assembly [Aspose.Tasks](../../../)


