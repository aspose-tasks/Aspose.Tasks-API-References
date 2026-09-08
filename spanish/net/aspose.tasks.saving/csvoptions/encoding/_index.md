---
title: "CsvOptions.Encoding"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad CsvOptions. Obtiene o establece una codificación con la que guardar CSV"
type: docs
weight: 30
url: /es/net/aspose.tasks.saving/csvoptions/encoding/
---
## CsvOptions.Encoding property

Obtiene o establece una codificación con la que guardar el CSV.

```csharp
public Encoding Encoding { get; set; }
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


