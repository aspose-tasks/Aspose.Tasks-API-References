---
title: "TaskLink.Equals"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode TaskLink. Retourne une valeur indiquant si cette instance est égale à un objet spécifié"
type: docs
weight: 90
url: /fr/net/aspose.tasks/tasklink/equals/
---
## Equals(TaskLink) {#equals}

Renvoie une valeur indiquant si cette instance est égale à un objet spécifié.

```csharp
public bool Equals(TaskLink other)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| other | TaskLink | L'instance spécifiée de la classe [`TaskLink`](../) à comparer avec cette instance. |

### Valeur de retour

**True** if the specified instance of the [`TaskLink`](../) class has the same predecessor and successor tasks as this instance; otherwise, **false**.

## Exemples

Montre comment vérifier l'égalité des liens de tâches.

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");

var link1 = project.TaskLinks[0];
var link2 = project.TaskLinks[1];

// L'égalité des liens de tâches est basée sur les tâches pred et succ.
Console.Write("Link 1 Pred: " + link1.PredTask.ToString());
Console.Write("Link 1 Succ: " + link1.SuccTask.ToString());
Console.Write("Link 2 Pred: " + link2.PredTask.ToString());
Console.Write("Link 2 Succ: " + link2.SuccTask.ToString());
Console.Write("Are task links equal: " + link1.Equals(link2));
```

### Voir aussi

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Renvoie une valeur indiquant si cette instance est égale à un objet spécifié.

```csharp
public override bool Equals(object obj)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| obj | Objet | L'objet à comparer avec cette instance. |

### Valeur de retour

**True** if the specified object is a TaskLink that has the same predecessor and successor as this instance; otherwise, **false**.

## Exemples

Montre comment vérifier l'égalité des liens de tâches.

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");

var link1 = project.TaskLinks[0];
var link2 = project.TaskLinks[1];

// L'égalité des liens de tâches est basée sur les tâches pred et succ.
Console.Write("Link 1 Pred: " + link1.PredTask.ToString());
Console.Write("Link 1 Succ: " + link1.SuccTask.ToString());
Console.Write("Link 2 Pred: " + link2.PredTask.ToString());
Console.Write("Link 2 Succ: " + link2.SuccTask.ToString());
Console.Write("Are task links equal: " + link1.Equals(link2));
```

### Voir aussi

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


