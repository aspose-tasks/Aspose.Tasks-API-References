---
title: "Prj.WorkFormat"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Prj. Le format utilisé pour afficher la durée de la tâche"
type: docs
weight: 790
url: /fr/net/aspose.tasks/prj/workformat/
---
## Prj.WorkFormat field

Le format utilisé pour afficher la durée de la tâche.

```csharp
public static readonly Key<TimeUnitType, PrjKey> WorkFormat;
```

## Exemples

Montre comment obtenir une durée avec le format de travail par défaut.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

Console.WriteLine("Project's work format: " + project.Get(Prj.WorkFormat));

// créer une valeur de travail avec le format de travail par défaut du projet
var work = project.GetWork(2);
Console.WriteLine("Work: " + work.TimeSpan);
Console.WriteLine("Time unit: " + work.TimeUnit);
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TimeUnitType](../../timeunittype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


