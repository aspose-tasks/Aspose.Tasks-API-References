---
title: "Tsk.CommitmentStart"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. La date de début d'une livraison. La lecture est prise en charge uniquement au format XML."
type: docs
weight: 180
url: /fr/net/aspose.tasks/tsk/commitmentstart/
---
## Tsk.CommitmentStart field

La date de début d'une livraison. Lecture prise en charge uniquement pour le format XML.

```csharp
public static readonly Key<DateTime, TaskKey> CommitmentStart;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.CommitmentStart.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.CommitmentStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Commitment Start: " + task.Get(Tsk.CommitmentStart));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


