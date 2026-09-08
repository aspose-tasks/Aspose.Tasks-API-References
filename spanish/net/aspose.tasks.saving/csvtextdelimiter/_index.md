---
title: "Enumeración CsvTextDelimiter"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Enumeración Aspose.Tasks.Saving.CsvTextDelimiter. Delimitador de texto para el formato CSV"
type: docs
weight: 1990
url: /es/net/aspose.tasks.saving/csvtextdelimiter/
---
## CsvTextDelimiter enumeration

Delimitador de texto para el formato CSV.

```csharp
public enum CsvTextDelimiter
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Comma | `0` | Delimitador de coma. |
| Semicolon | `1` | Delimitador de punto y coma. |
| Space | `2` | Delimitador de espacio. |
| Tab | `3` | Delimitador de tabulación. |

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


