---
title: "Classe LevelingOptions"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.Leveling.LevelingOptions. Permet de spécifier les paramètres du nivellement des ressources"
type: docs
weight: 940
url: /fr/net/aspose.tasks.leveling/levelingoptions/
---
## LevelingOptions class

Permet de spécifier les paramètres du nivellement des ressources.

```csharp
public sealed class LevelingOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [LevelingOptions](levelingoptions/)() | Initialise une nouvelle instance de la classe `LevelingOptions`. |

## Propriétés

| Nom | Description |
| --- | --- |
| [CancellationToken](../../aspose.tasks.leveling/levelingoptions/cancellationtoken/) { get; set; } | Obtient ou définit un jeton qui peut être utilisé pour annuler une opération de nivellement du projet. |
| [FinishDate](../../aspose.tasks.leveling/levelingoptions/finishdate/) { get; set; } | Obtient ou définit la date de fin de la période de nivellement. La valeur par défaut est la date de fin du projet. |
| [LevelingOrder](../../aspose.tasks.leveling/levelingoptions/levelingorder/) { get; set; } | Obtient l'ordre dans lequel l'algorithme de nivellement retarde les tâches présentant des surallocations. Après la détermination des tâches à l'origine de la surallocation et des tâches pouvant être retardées, l'ordre spécifié indique quelle tâche doit être retardée en premier. |
| [MessageHandler](../../aspose.tasks.leveling/levelingoptions/messagehandler/) { get; set; } | Obtient ou définit le rappel du gestionnaire de messages qui peut être utilisé pour intercepter les messages de journal produits par Aspose.Tasks lors du nivellement des ressources. |
| [MessageLevel](../../aspose.tasks.leveling/levelingoptions/messagelevel/) { get; set; } | Obtient ou définit le niveau des messages de journal émis par Aspose.Tasks pendant le nivellement des ressources. |
| [Resources](../../aspose.tasks.leveling/levelingoptions/resources/) { get; set; } | Obtient ou définit la liste des ressources qui seront nivelées. Si null est défini, toutes les ressources du projet seront nivelées. |
| [StartDate](../../aspose.tasks.leveling/levelingoptions/startdate/) { get; set; } | Obtient ou définit la date de début de la période de nivellement. La valeur par défaut est la date de début du projet. |

## Exemples

Montre comment niveler une ressource spécifique, personnaliser les options de nivellement et examiner les messages de l'algorithme de nivellement.

```csharp
var project = new Project(DataDir + "Software Development Plan.mpp");

var levelingOptions = new LevelingOptions();
levelingOptions.StartDate = new DateTime(2013, 3, 10);
levelingOptions.FinishDate = new DateTime(2013, 4, 30);
levelingOptions.Resources = new List<Resource> { project.Resources.GetById(7) };
levelingOptions.MessageLevel = MessageLevel.Information;
levelingOptions.MessageHandler = new LevelingMessageHandler();

ResourceLeveler.LevelResources(project, levelingOptions);
```

### Voir aussi

* namespace [Aspose.Tasks.Leveling](../../aspose.tasks.leveling/)
* assembly [Aspose.Tasks](../../)


