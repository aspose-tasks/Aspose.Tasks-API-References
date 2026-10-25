---
title: "Task.Equals"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método de Task. Devuelve un valor que indica si esta instancia es igual a una tarea especificada"
type: docs
weight: 1330
url: /es/net/aspose.tasks/task/equals/
---
## Equals(Task) {#equals}

Devuelve un valor que indica si esta instancia es igual a una tarea especificada.

```csharp
public bool Equals(Task other)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| otro | Tarea | La tarea especificada para comparar con esta instancia. |

### Valor devuelto

devuelve true si la tarea especificada y esta instancia tienen identificadores únicos iguales.

## Ejemplos

Muestra cómo iterar sobre las asignaciones de la tarea.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);
foreach (var task in collector.Tasks)
{
    // mostrar asignaciones de la tarea
    foreach (var assignment in task.Assignments)
    {
        Console.WriteLine(assignment.ToString());
    }
}
```

### Ver también

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Devuelve un valor que indica si esta instancia es igual a un objeto especificado.

```csharp
public override bool Equals(object obj)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | Objeto | El objeto especificado para comparar con esta instancia. |

### Valor devuelto

devuelve true si la tarea especificada y esta instancia tienen identificadores únicos iguales.

## Ejemplos

Muestra cómo iterar sobre las asignaciones de la tarea.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);
foreach (var task in collector.Tasks)
{
    // mostrar asignaciones de la tarea
    foreach (var assignment in task.Assignments)
    {
        Console.WriteLine(assignment.ToString());
    }
}
```

### Ver también

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


