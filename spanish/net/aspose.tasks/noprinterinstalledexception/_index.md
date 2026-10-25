---
title: "Clase NoPrinterInstalledException"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.NoPrinterInstalledException. Representa una excepción que se lanza cuando no hay una impresora instalada en el sistema operativo."
type: docs
weight: 1100
url: /es/net/aspose.tasks/noprinterinstalledexception/
---
## NoPrinterInstalledException class

Representa una excepción que se lanza cuando no hay impresora instalada en el sistema operativo.

```csharp
public class NoPrinterInstalledException : Exception
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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


