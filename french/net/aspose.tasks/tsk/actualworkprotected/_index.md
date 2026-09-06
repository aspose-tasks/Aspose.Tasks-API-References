---
title: "Tsk.ActualWorkProtected"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. La durée pendant laquelle le travail réel est protégé. La lecture n'est prise en charge que pour le format XML"
type: docs
weight: 100
url: /fr/net/aspose.tasks/tsk/actualworkprotected/
---
## Tsk.ActualWorkProtected field

La durée pendant laquelle le travail réel est protégé. Lecture prise en charge uniquement pour le format XML.

```csharp
public static readonly Key<Duration, TaskKey> ActualWorkProtected;
```

## Exemples

Montre comment lire/écrire la propriété Tsk.ActualWorkProtected.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualWorkProtected, project.GetWork(1));

Console.WriteLine("Actual Work Protected: " + task.Get(Tsk.ActualWorkProtected));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


