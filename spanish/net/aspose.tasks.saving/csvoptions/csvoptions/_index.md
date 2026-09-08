---
title: "CsvOptions.CsvOptions"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Constructor CsvOptions. Inicializa una nueva instancia de la clase CsvOptions que puede usarse para guardar el proyecto en formato CSV"
type: docs
weight: 10
url: /es/net/aspose.tasks.saving/csvoptions/csvoptions/
---
## CsvOptions constructor

Inicializa una nueva instancia de la clase [`CsvOptions`](../) que puede usarse para guardar el proyecto en formato CSV.

```csharp
public CsvOptions()
```

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

* class [CsvOptions](../)
* namespace [Aspose.Tasks.Saving](../../csvoptions/)
* assembly [Aspose.Tasks](../../../)


