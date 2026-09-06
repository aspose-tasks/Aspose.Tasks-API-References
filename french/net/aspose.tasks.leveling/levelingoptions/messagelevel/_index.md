---
title: "LevelingOptions.MessageLevel"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété LevelingOptions. Obtient ou définit le niveau des messages de journal émis par Aspose.Tasks pendant le nivellement des ressources"
type: docs
weight: 60
url: /fr/net/aspose.tasks.leveling/levelingoptions/messagelevel/
---
## LevelingOptions.MessageLevel property

Obtient ou définit le niveau des messages de journal émis par Aspose.Tasks pendant le nivellement des ressources.

```csharp
public MessageLevel MessageLevel { get; set; }
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

* enum [MessageLevel](../../../aspose.tasks/messagelevel/)
* class [LevelingOptions](../)
* namespace [Aspose.Tasks.Leveling](../../levelingoptions/)
* assembly [Aspose.Tasks](../../../)


