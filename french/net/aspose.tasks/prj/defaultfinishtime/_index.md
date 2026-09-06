---
title: "Prj.DefaultFinishTime"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Prj. Le temps de fin par défaut des nouvelles tâches"
type: docs
weight: 230
url: /fr/net/aspose.tasks/prj/defaultfinishtime/
---
## Prj.DefaultFinishTime field

L'heure de fin par défaut des nouvelles tâches.

```csharp
public static readonly Key<DateTime, PrjKey> DefaultFinishTime;
```

## Exemples

Montre comment lire/écrire la propriété Prj.DefaultFinishTime.

```csharp
var project = new Project();

project.Set(Prj.DefaultFinishTime, new DateTime(2000, 1, 3, 10, 0, 0));

Console.WriteLine("Default Finish Time: " + project.Get(Prj.DefaultFinishTime));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


