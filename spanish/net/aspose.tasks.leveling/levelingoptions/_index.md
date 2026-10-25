---
title: "Clase LevelingOptions"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.Leveling.LevelingOptions. Permite especificar los parámetros del nivelado de recursos"
type: docs
weight: 940
url: /es/net/aspose.tasks.leveling/levelingoptions/
---
## LevelingOptions class

Permite especificar parámetros del nivelado de recursos.

```csharp
public sealed class LevelingOptions
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [LevelingOptions](levelingoptions/)() | Inicializa una nueva instancia de la clase `LevelingOptions`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [CancellationToken](../../aspose.tasks.leveling/levelingoptions/cancellationtoken/) { get; set; } | Obtiene o establece un token que puede usarse para cancelar una operación de nivelado del proyecto. |
| [FinishDate](../../aspose.tasks.leveling/levelingoptions/finishdate/) { get; set; } | Obtiene o establece la fecha de finalización del período de nivelado. El valor predeterminado es la fecha de finalización del proyecto. |
| [LevelingOrder](../../aspose.tasks.leveling/levelingoptions/levelingorder/) { get; set; } | Obtiene el orden en que el algoritmo de nivelado retrasa las tareas que tienen sobreasignaciones. Después de determinar las tareas que causan la sobreasignación y qué tareas pueden retrasarse, se utiliza el orden especificado para decidir cuál tarea debe retrasarse primero. |
| [MessageHandler](../../aspose.tasks.leveling/levelingoptions/messagehandler/) { get; set; } | Obtiene o establece la devolución de llamada del manejador de mensajes que puede usarse para interceptar los mensajes de registro generados por Aspose.Tasks durante el nivelado de recursos. |
| [MessageLevel](../../aspose.tasks.leveling/levelingoptions/messagelevel/) { get; set; } | Obtiene o establece el nivel de los mensajes de registro emitidos por Aspose.Tasks durante el nivelado de recursos. |
| [Resources](../../aspose.tasks.leveling/levelingoptions/resources/) { get; set; } | Obtiene o establece la lista de recursos que serán nivelados. Si se establece null, todos los recursos del proyecto serán nivelados. |
| [StartDate](../../aspose.tasks.leveling/levelingoptions/startdate/) { get; set; } | Obtiene o establece la fecha de inicio del período de nivelado. El valor predeterminado es la fecha de inicio del proyecto. |

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

* namespace [Aspose.Tasks.Leveling](../../aspose.tasks.leveling/)
* assembly [Aspose.Tasks](../../)


