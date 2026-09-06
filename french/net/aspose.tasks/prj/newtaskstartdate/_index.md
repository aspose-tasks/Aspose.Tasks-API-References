---
title: "Prj.NewTaskStartDate"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Prj. Le type de date de début par défaut pour les nouvelles tâches"
type: docs
weight: 580
url: /fr/net/aspose.tasks/prj/newtaskstartdate/
---
## Prj.NewTaskStartDate field

Le type de date de début par défaut pour les nouvelles tâches.

```csharp
public static readonly Key<TaskStartDateType, PrjKey> NewTaskStartDate;
```

## Exemples

Montre comment définir les attributs pour les nouvelles tâches.

```csharp
var project = new Project();
project.Set(Prj.NewTaskStartDate, TaskStartDateType.CurrentDate);

Console.WriteLine("New Task Start Date: " + project.Get(Prj.NewTaskStartDate));
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskStartDateType](../../taskstartdatetype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


