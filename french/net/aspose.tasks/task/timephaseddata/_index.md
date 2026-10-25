---
title: "Task.TimephasedData"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété Task. Obtient ou définit un objet TimephasedDataCollection de cette tâche. Le bloc de données temporelles associé à une tâche"
type: docs
weight: 1220
url: /fr/net/aspose.tasks/task/timephaseddata/
---
## Task.TimephasedData property

Obtient ou définit un objet TimephasedDataCollection de cette tâche. Le bloc de données temporelles associé à une tâche.

```csharp
public TimephasedDataCollection TimephasedData { get; set; }
```

## Remarques

Lecture prise en charge uniquement au format XML.

## Exemples

Montre comment itérer sur les données temporelles d'une tâche.

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");
var task = project.RootTask.Children.GetById(1);

foreach (var td in task.TimephasedData)
{
    Console.WriteLine("Start: " + td.Start);
    Console.WriteLine("Finish: " + td.Finish);
    Console.WriteLine("Type: " + td.TimephasedDataType);
}
```

### Voir aussi

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


