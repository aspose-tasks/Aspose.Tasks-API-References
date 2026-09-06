---
title: "Enum TaskStartDateType"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Aspose.Tasks.TaskStartDateType enum. Spécifie le type de la date de début d'une tâche"
type: docs
weight: 2450
url: /fr/net/aspose.tasks/taskstartdatetype/
---
## TaskStartDateType enumeration

Spécifie le type de la date de début d'une tâche.

```csharp
public enum TaskStartDateType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Undefined | `-1` | La valeur du champ n'était pas définie dans le fichier de projet original. |
| ProjectStartDate | `0` | Date de début du projet |
| CurrentDate | `1` | Date actuelle |

## Remarques

Lors de l'exportation vers XML, les valeurs Undefined seront éliminées du XML résultant.

## Exemples

Montre comment définir la date de début par défaut d'une tâche comme 'CurrentDate'.

```csharp
var project = new Project();
project.Set(Prj.NewTaskStartDate, TaskStartDateType.CurrentDate);
project.Save(OutDir + "SetAttributesForNewTasks_out.xml", SaveFileFormat.Xml);
```

### Voir aussi

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


