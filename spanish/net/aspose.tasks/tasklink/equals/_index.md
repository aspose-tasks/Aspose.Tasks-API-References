---
title: "TaskLink.Equals"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método TaskLink. Devuelve un valor que indica si esta instancia es igual a un objeto especificado"
type: docs
weight: 90
url: /es/net/aspose.tasks/tasklink/equals/
---
## Equals(TaskLink) {#equals}

Devuelve un valor que indica si esta instancia es igual a un objeto especificado.

```csharp
public bool Equals(TaskLink other)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| other | TaskLink | La instancia especificada de la clase [`TaskLink`](../) para comparar con esta instancia. |

### Valor devuelto

**True** if the specified instance of the [`TaskLink`](../) class has the same predecessor and successor tasks as this instance; otherwise, **false**.

## Ejemplos

Muestra cómo comprobar la igualdad de los enlaces de tareas.

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");

var link1 = project.TaskLinks[0];
var link2 = project.TaskLinks[1];

// La igualdad de los enlaces de tareas se basa en las tareas pred y succ.
Console.Write("Link 1 Pred: " + link1.PredTask.ToString());
Console.Write("Link 1 Succ: " + link1.SuccTask.ToString());
Console.Write("Link 2 Pred: " + link2.PredTask.ToString());
Console.Write("Link 2 Succ: " + link2.SuccTask.ToString());
Console.Write("Are task links equal: " + link1.Equals(link2));
```

### Ver también

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Devuelve un valor que indica si esta instancia es igual a un objeto especificado.

```csharp
public override bool Equals(object obj)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | Objeto | El objeto para comparar con esta instancia. |

### Valor devuelto

**True** if the specified object is a TaskLink that has the same predecessor and successor as this instance; otherwise, **false**.

## Ejemplos

Muestra cómo comprobar la igualdad de los enlaces de tareas.

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");

var link1 = project.TaskLinks[0];
var link2 = project.TaskLinks[1];

// La igualdad de los enlaces de tareas se basa en las tareas pred y succ.
Console.Write("Link 1 Pred: " + link1.PredTask.ToString());
Console.Write("Link 1 Succ: " + link1.SuccTask.ToString());
Console.Write("Link 2 Pred: " + link2.PredTask.ToString());
Console.Write("Link 2 Succ: " + link2.SuccTask.ToString());
Console.Write("Are task links equal: " + link1.Equals(link2));
```

### Ver también

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


