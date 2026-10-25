---
title: "PrintOptions.PrintOptions"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Constructor de PrintOptions. Inicializa una nueva instancia de la clase PrintOptions que puede usarse para establecer diferentes opciones al imprimir el proyecto"
type: docs
weight: 10
url: /es/net/aspose.tasks.saving/printoptions/printoptions/
---
## PrintOptions constructor

Inicializa una nueva instancia de la clase [`PrintOptions`](../) que puede usarse para establecer diferentes opciones al imprimir el proyecto.

```csharp
public PrintOptions()
```

## Ejemplos

Muestra cómo usar las opciones de impresión.

```csharp
try
{
    var project = new Project(DataDir + "Project2.mpp");
    var options = new PrintOptions
    {
        Timescale = Timescale.ThirdsOfMonths
    };
    if (project.GetPageCount(Timescale.ThirdsOfMonths) <= 280)
    {
        project.Print(options);
    }
}
catch (NoPrinterInstalledException ex)
{
    Console.WriteLine(ex.Message);
}
```

### Ver también

* class [PrintOptions](../)
* namespace [Aspose.Tasks.Saving](../../printoptions/)
* assembly [Aspose.Tasks](../../../)


