---
title: "Enumeración DataCategory"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Enumeración Aspose.Tasks.Saving.DataCategory. La categoría de datos utilizada al guardar en CSV."
type: docs
weight: 2000
url: /es/net/aspose.tasks.saving/datacategory/
---
## DataCategory enumeration

La categoría de datos utilizada al guardar en CSV.

```csharp
public enum DataCategory
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Tasks | `0` | Información de tareas. |
| Resources | `1` | Información de recursos. |
| Assignments | `2` | Información de asignaciones. |

## Ejemplos

Muestra cómo usar &lt;see cref="Aspose.Tasks.Saving.CsvOptions" /&gt; para guardar un proyecto como archivo CSV.

```csharp
var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");
var options = new CsvOptions
{
    DataCategory = DataCategory.Resources,
    TextDelimiter = CsvTextDelimiter.Semicolon,
    Encoding = Encoding.Unicode, IncludeHeaders = true
};

project.Save(OutDir + "WorkWithCsvOptions_out.csv", options);
```

### Ver también

* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


