---
title: "LevelingOptions.MessageHandler"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "LevelingOptions-Eigenschaft. Gibt den Rückruf für den Nachrichten-Handler zurück oder legt ihn fest, der verwendet werden kann, um von Aspose.Tasks während der Ressourcenlevelung erzeugte Protokollnachrichten abzufangen."
type: docs
weight: 50
url: /de/net/aspose.tasks.leveling/levelingoptions/messagehandler/
---
## LevelingOptions.MessageHandler property

Ruft den Nachrichten-Handler-Callback ab oder legt ihn fest, der verwendet werden kann, um Protokollnachrichten von Aspose.Tasks während des Ressourcen-Levelings abzufangen.

```csharp
public IMessageHandler MessageHandler { get; set; }
```

## Beispiele

Zeigt, wie man eine bestimmte Ressource ausgleicht, Ausgleichsoptionen anpasst und Nachrichten des Ausgleichsalgorithmus untersucht.

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

### Siehe auch

* interface [IMessageHandler](../../../aspose.tasks/imessagehandler/)
* class [LevelingOptions](../)
* namespace [Aspose.Tasks.Leveling](../../levelingoptions/)
* assembly [Aspose.Tasks](../../../)


