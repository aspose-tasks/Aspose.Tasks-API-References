---
title: "Interface IMessageHandler"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Interface Aspose.Tasks.IMessageHandler. Représente un rappel des résultats du nivellement des ressources"
type: docs
weight: 880
url: /fr/net/aspose.tasks/imessagehandler/
---
## IMessageHandler interface

Représente un rappel des résultats de l’étalonnage des ressources.

```csharp
public interface IMessageHandler
```

## Méthodes

| Nom | Description |
| --- | --- |
| [Message](../../aspose.tasks/imessagehandler/message/)(MessageLevel, string) | Aspose.Tasks invoque cette méthode lorsqu'il génère un message. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


