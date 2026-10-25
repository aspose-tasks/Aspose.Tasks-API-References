---
title: "Tsk.ActivityId"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Champ Tsk. Représente le champ d'identifiant d'activité, l'identifiant unique d'une tâche utilisé par Primavera. Applicable uniquement aux projets Primavera."
type: docs
weight: 10
url: /fr/net/aspose.tasks/tsk/activityid/
---
## Tsk.ActivityId field

Représente le champ d'identifiant d'activité - l'identifiant unique d'une tâche utilisé par Primavera. (uniquement applicable aux projets Primavera).

```csharp
public static readonly Key<string, TaskKey> ActivityId;
```

## Exemples

Montre comment travailler avec le champ ActivityId spécifique aux projets Primavera.

```csharp
var project = new Project(DataDir + "test.xer");

var task = project.RootTask.Children.GetById(1);

Console.WriteLine("Task activity_id: {0}", task.Get(Tsk.ActivityId));

task.Set(Tsk.ActivityId, "CUSTOM_ACTIVITY_ID");

// Créez des options d'enregistrement Primavera et spécifiez que les ActivityIds ne doivent pas être écrasés lors de l'enregistrement.
var options = new PrimaveraSaveOptions
{
    RenumberActivityIds = false
};

project.Save(OutDir + "WorkWithPrimaveraActivityId_out.xer", options);
```

### Voir aussi

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


