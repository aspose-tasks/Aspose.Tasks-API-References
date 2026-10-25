---
title: "TaskLink.Equals"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "TaskLink metodo. Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato"
type: docs
weight: 90
url: /it/net/aspose.tasks/tasklink/equals/
---
## Equals(TaskLink) {#equals}

Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato.

```csharp
public bool Equals(TaskLink other)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| other | TaskLink | L'istanza specificata della classe [`TaskLink`](../) da confrontare con questa istanza. |

### Valore di ritorno

**True** if the specified instance of the [`TaskLink`](../) class has the same predecessor and successor tasks as this instance; otherwise, **false**.

## Esempi

Mostra come verificare l'uguaglianza dei collegamenti di attività.

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");

var link1 = project.TaskLinks[0];
var link2 = project.TaskLinks[1];

// L'uguaglianza dei collegamenti di attività si basa sui task pred e succ.
Console.Write("Link 1 Pred: " + link1.PredTask.ToString());
Console.Write("Link 1 Succ: " + link1.SuccTask.ToString());
Console.Write("Link 2 Pred: " + link2.PredTask.ToString());
Console.Write("Link 2 Succ: " + link2.SuccTask.ToString());
Console.Write("Are task links equal: " + link1.Equals(link2));
```

### Vedi anche

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato.

```csharp
public override bool Equals(object obj)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | Oggetto | L'oggetto da confrontare con questa istanza. |

### Valore di ritorno

**True** if the specified object is a TaskLink that has the same predecessor and successor as this instance; otherwise, **false**.

## Esempi

Mostra come verificare l'uguaglianza dei collegamenti di attività.

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");

var link1 = project.TaskLinks[0];
var link2 = project.TaskLinks[1];

// L'uguaglianza dei collegamenti di attività si basa sui task pred e succ.
Console.Write("Link 1 Pred: " + link1.PredTask.ToString());
Console.Write("Link 1 Succ: " + link1.SuccTask.ToString());
Console.Write("Link 2 Pred: " + link2.PredTask.ToString());
Console.Write("Link 2 Succ: " + link2.SuccTask.ToString());
Console.Write("Are task links equal: " + link1.Equals(link2));
```

### Vedi anche

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


