---
title: "Tsk.CommitmentFinish"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. La date de fin d'une livraison.  Lecture prise en charge uniquement pour le format XML"
type: docs
weight: 170
url: /fr/net/aspose.tasks/tsk/commitmentfinish/
---
## Tsk.CommitmentFinish field

La date de fin d'une livraison. Lecture prise en charge uniquement pour le format XML.

```csharp
public static readonly Key<DateTime, TaskKey> CommitmentFinish;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.CommitmentFinish.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.CommitmentFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Commitment Finish: " + task.Get(Tsk.CommitmentFinish));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


