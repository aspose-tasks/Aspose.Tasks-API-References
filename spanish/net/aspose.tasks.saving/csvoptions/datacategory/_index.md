---
title: "CsvOptions.DataCategory"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad CsvOptions. Obtiene o establece una categoría de datos que se guardará"
type: docs
weight: 20
url: /es/net/aspose.tasks.saving/csvoptions/datacategory/
---
## CsvOptions.DataCategory property

Obtiene o establece una categoría de datos que se guardará.

```csharp
public DataCategory DataCategory { get; set; }
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

* enum [DataCategory](../../datacategory/)
* class [CsvOptions](../)
* namespace [Aspose.Tasks.Saving](../../csvoptions/)
* assembly [Aspose.Tasks](../../../)


