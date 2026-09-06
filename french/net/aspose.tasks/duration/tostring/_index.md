---
title: "Duration.ToString"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode Duration. Renvoie une représentation sous forme de chaîne de cette instance"
type: docs
weight: 120
url: /fr/net/aspose.tasks/duration/tostring/
---
## Duration.ToString method

Renvoie une représentation sous forme de chaîne de cette instance.

```csharp
public override string ToString()
```

### Valeur de retour

une représentation sous forme de chaîne de cette instance.

## Exemples

Montre comment convertir une durée en chaîne.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");
var task = project.RootTask.Children.GetById(1);

// obtenir la durée de la tâche
var duration = task.Get(Tsk.Duration);
Console.WriteLine("The duration as a string: " + duration.ToString());
```

### Voir aussi

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


