---
title: "ResourceLeveler.LevelResources"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "ResourceLeveler-Methode. Levelt Aufgaben für die angegebenen Ressourcen mit den angegebenen Ebenungsoptionen."
type: docs
weight: 30
url: /de/net/aspose.tasks.leveling/resourceleveler/levelresources/
---
## ResourceLeveler.LevelResources method

Levelt Aufgaben für die angegebenen Ressourcen mit den angegebenen Leveling-Optionen.

```csharp
public static LevelingResult LevelResources(Project project, LevelingOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Projekt | Projekt | Projekt zum Anwenden der Ressourcenebenen. |
| Optionen | LevelingOptions | Optionen, die festlegen, wie Ressourcen geebnet werden. |

### Rückgabewert

Objekt, das die Ergebnisse der Ressourcenebene enthält.

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | wenn Parameter options null ist. |

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

* class [LevelingResult](../../levelingresult/)
* class [Project](../../../aspose.tasks/project/)
* class [LevelingOptions](../../levelingoptions/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)


