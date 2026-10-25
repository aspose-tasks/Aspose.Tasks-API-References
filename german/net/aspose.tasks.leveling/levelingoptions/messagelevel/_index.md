---
title: "LevelingOptions.MessageLevel"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "LevelingOptions-Eigenschaft. Gibt das Niveau der von Aspose.Tasks während der Ressourcenlevelung ausgegebenen Protokollnachrichten zurück oder legt es fest."
type: docs
weight: 60
url: /de/net/aspose.tasks.leveling/levelingoptions/messagelevel/
---
## LevelingOptions.MessageLevel property

Ruft das Protokoll-Level der von Aspose.Tasks während des Ressourcen-Levelings ausgegebenen Nachrichten ab oder legt es fest.

```csharp
public MessageLevel MessageLevel { get; set; }
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

* enum [MessageLevel](../../../aspose.tasks/messagelevel/)
* class [LevelingOptions](../)
* namespace [Aspose.Tasks.Leveling](../../levelingoptions/)
* assembly [Aspose.Tasks](../../../)


