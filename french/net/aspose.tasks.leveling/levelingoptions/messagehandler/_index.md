---
title: "LevelingOptions.MessageHandler"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété LevelingOptions. Obtient ou définit le rappel du gestionnaire de messages qui peut être utilisé pour intercepter les messages de journal produits par Aspose.Tasks pendant le nivellement des ressources"
type: docs
weight: 50
url: /fr/net/aspose.tasks.leveling/levelingoptions/messagehandler/
---
## LevelingOptions.MessageHandler property

Obtient ou définit le rappel du gestionnaire de messages qui peut être utilisé pour intercepter les messages de journal produits par Aspose.Tasks lors du nivellement des ressources.

```csharp
public IMessageHandler MessageHandler { get; set; }
```

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

* interface [IMessageHandler](../../../aspose.tasks/imessagehandler/)
* class [LevelingOptions](../)
* namespace [Aspose.Tasks.Leveling](../../levelingoptions/)
* assembly [Aspose.Tasks](../../../)


