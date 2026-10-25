---
title: "ResourceLeveler.LevelResources"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método ResourceLeveler. Niveliza tareas para los recursos especificados usando las opciones de nivelación especificadas."
type: docs
weight: 30
url: /es/net/aspose.tasks.leveling/resourceleveler/levelresources/
---
## ResourceLeveler.LevelResources method

Nivela las tareas de los recursos especificados usando las opciones de nivelado especificadas.

```csharp
public static LevelingResult LevelResources(Project project, LevelingOptions options)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| project | Project | Proyecto al que se aplicará la nivelación de recursos. |
| opciones | LevelingOptions | Opciones que especifican cómo nivelar los recursos. |

### Valor devuelto

Objeto que contiene los resultados de la nivelación de recursos.

### Excepciones

| excepción | condición |
| --- | --- |
| ArgumentNullException | si el parámetro options es nulo. |

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

* class [LevelingResult](../../levelingresult/)
* class [Project](../../../aspose.tasks/project/)
* class [LevelingOptions](../../levelingoptions/)
* class [ResourceLeveler](../)
* namespace [Aspose.Tasks.Leveling](../../resourceleveler/)
* assembly [Aspose.Tasks](../../../)


