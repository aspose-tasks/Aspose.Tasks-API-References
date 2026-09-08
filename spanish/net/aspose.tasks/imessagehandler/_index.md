---
title: "Interfaz IMessageHandler"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Interfaz Aspose.Tasks.IMessageHandler. Representa una devolución de llamada de los resultados del nivelado de recursos"
type: docs
weight: 880
url: /es/net/aspose.tasks/imessagehandler/
---
## IMessageHandler interface

Representa una devolución de llamada con los resultados del nivelado de recursos.

```csharp
public interface IMessageHandler
```

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Message](../../aspose.tasks/imessagehandler/message/)(MessageLevel, string) | Aspose.Tasks invoca este método cuando genera un mensaje. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


