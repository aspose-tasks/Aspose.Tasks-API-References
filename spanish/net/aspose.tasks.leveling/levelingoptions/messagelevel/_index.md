---
title: "LevelingOptions.MessageLevel"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad LevelingOptions. Obtiene o establece el nivel de los mensajes de registro emitidos por Aspose.Tasks durante el nivelado de recursos"
type: docs
weight: 60
url: /es/net/aspose.tasks.leveling/levelingoptions/messagelevel/
---
## LevelingOptions.MessageLevel property

Obtiene o establece el nivel de los mensajes de registro emitidos por Aspose.Tasks durante el nivelado de recursos.

```csharp
public MessageLevel MessageLevel { get; set; }
```

## Ejemplos

Muestra cómo nivelar un recurso específico, personalizar las opciones de nivelación y examinar los mensajes del algoritmo de nivelación.

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

### Ver también

* enum [MessageLevel](../../../aspose.tasks/messagelevel/)
* class [LevelingOptions](../)
* namespace [Aspose.Tasks.Leveling](../../levelingoptions/)
* assembly [Aspose.Tasks](../../../)


