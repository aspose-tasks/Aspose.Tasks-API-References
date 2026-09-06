---
title: "ResourceLeveler.LevelResources"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode ResourceLeveler. Nivele les tâches pour les ressources spécifiées en utilisant les options de nivellement spécifiées."
type: docs
weight: 30
url: /fr/net/aspose.tasks.leveling/resourceleveler/levelresources/
---
## ResourceLeveler.LevelResources method

Nivele les tâches pour les ressources spécifiées en utilisant les options de nivellement spécifiées.

```csharp
public static LevelingResult LevelResources(Project project, LevelingOptions options)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| project | Project | Projet auquel appliquer le nivellement des ressources. |
| options | LevelingOptions | Options qui spécifient comment niveler les ressources. |

### Valeur de retour

Objet contenant les résultats du nivellement des ressources.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | si le paramètre options est nul. |

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

* class [LevelingResult](../../levelingresult/)
* class [Project](../../../aspose.tasks/project/)
* class [LevelingOptions](../../levelingoptions/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)


