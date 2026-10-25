---
title: "ResourceAssignmentCollection.Add"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método ResourceAssignmentCollection. Añade una nueva asignación a la ResourceAssignmentCollection"
type: docs
weight: 50
url: /es/net/aspose.tasks/resourceassignmentcollection/add/
---
## Add(Task, Resource, double) {#add_1}

Agrega una nueva asignación a ResourceAssignmentCollection.

```csharp
public ResourceAssignment Add(Task task, Resource resource, double units)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| tarea | Tarea | Una tarea para asignar. |
| recurso | Recurso | Un recurso para asignar. |
| unidades | Double | El número de unidades para una nueva asignación. |

### Valor devuelto

Asignación añadida.

## Ejemplos

Muestra cómo trabajar con colecciones de asignaciones de recursos.

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

// trabajar con asignaciones...
Console.WriteLine("Is resource assignment collection read-only?: " + project.ResourceAssignments.IsReadOnly);

// convertir la colección en una lista
List<ResourceAssignment> resourceAssignments = project.ResourceAssignments.ToList();

// iterar sobre la lista
foreach (var ra in resourceAssignments)
{
    Console.WriteLine(ra.ToString());
}
```

### Ver también

* class [ResourceAssignment](../../resourceassignment/)
* class [Task](../../task/)
* class [Resource](../../resource/)
* class [ResourceAssignmentCollection](../)
* namespace [Aspose.Tasks](../../resourceassignmentcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(Task, Resource, decimal) {#add_2}

Agrega una nueva asignación a ResourceAssignmentCollection.

```csharp
public ResourceAssignment Add(Task task, Resource resource, decimal cost)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| tarea | Tarea | Una tarea para asignar. |
| recurso | Recurso | Un recurso de costo para asignar. |
| costo | Decimal | El costo de una nueva asignación. |

### Valor devuelto

Asignación añadida.

## Ejemplos

Muestra cómo trabajar con colecciones de asignaciones de recursos.

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

// trabajar con asignaciones...
Console.WriteLine("Is resource assignment collection read-only?: " + project.ResourceAssignments.IsReadOnly);

// convertir la colección en una lista
List<ResourceAssignment> resourceAssignments = project.ResourceAssignments.ToList();

// iterar sobre la lista
foreach (var ra in resourceAssignments)
{
    Console.WriteLine(ra.ToString());
}
```

### Ver también

* class [ResourceAssignment](../../resourceassignment/)
* class [Task](../../task/)
* class [Resource](../../resource/)
* class [ResourceAssignmentCollection](../)
* namespace [Aspose.Tasks](../../resourceassignmentcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(Task, Resource) {#add}

Agrega una nueva asignación a ResourceAssignmentCollection.

```csharp
public ResourceAssignment Add(Task task, Resource resource)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| tarea | Tarea | Una tarea para asignar. |
| recurso | Recurso | Un recurso para asignar. |

### Valor devuelto

Asignación añadida.

## Ejemplos

Muestra cómo trabajar con colecciones de asignaciones de recursos.

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

// trabajar con asignaciones...
Console.WriteLine("Is resource assignment collection read-only?: " + project.ResourceAssignments.IsReadOnly);

// convertir la colección en una lista
List<ResourceAssignment> resourceAssignments = project.ResourceAssignments.ToList();

// iterar sobre la lista
foreach (var ra in resourceAssignments)
{
    Console.WriteLine(ra.ToString());
}
```

### Ver también

* class [ResourceAssignment](../../resourceassignment/)
* class [Task](../../task/)
* class [Resource](../../resource/)
* class [ResourceAssignmentCollection](../)
* namespace [Aspose.Tasks](../../resourceassignmentcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(ResourceAssignment) {#add_3}

Esta es la implementación de referencia del método Add de ICollection, que solo lanza NotSupportedException

```csharp
public void Add(ResourceAssignment item)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| elemento | ResourceAssignment | El elemento a eliminar. |

### Ver también

* class [ResourceAssignment](../../resourceassignment/)
* class [ResourceAssignmentCollection](../)
* namespace [Aspose.Tasks](../../resourceassignmentcollection/)
* assembly [Aspose.Tasks](../../../)


