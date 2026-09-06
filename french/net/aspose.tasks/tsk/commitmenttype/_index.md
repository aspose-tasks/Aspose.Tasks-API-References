---
title: "Tsk.CommitmentType"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Détermine si une tâche possède une livraison associée ou une dépendance à une livraison associée. La lecture est prise en charge uniquement au format XML."
type: docs
weight: 190
url: /fr/net/aspose.tasks/tsk/commitmenttype/
---
## Tsk.CommitmentType field

Détermine si une tâche possède une livraison associée ou une dépendance à une livraison associée. Lecture prise en charge uniquement pour le format XML.

```csharp
public static readonly Key<int, TaskKey> CommitmentType;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.CommitmentType.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.CommitmentType, 2);

Console.WriteLine("Commitment Type: " + task.Get(Tsk.CommitmentType));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


