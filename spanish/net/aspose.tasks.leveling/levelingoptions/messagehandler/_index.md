---
title: "LevelingOptions.MessageHandler"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad LevelingOptions. Obtiene o establece la devolución de llamada del manejador de mensajes que puede usarse para interceptar los mensajes de registro producidos por Aspose.Tasks durante el nivelado de recursos"
type: docs
weight: 50
url: /es/net/aspose.tasks.leveling/levelingoptions/messagehandler/
---
## LevelingOptions.MessageHandler property

Obtiene o establece la devolución de llamada del manejador de mensajes que puede usarse para interceptar los mensajes de registro generados por Aspose.Tasks durante el nivelado de recursos.

```csharp
public IMessageHandler MessageHandler { get; set; }
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

* interface [IMessageHandler](../../../aspose.tasks/imessagehandler/)
* class [LevelingOptions](../)
* namespace [Aspose.Tasks.Leveling](../../levelingoptions/)
* assembly [Aspose.Tasks](../../../)


