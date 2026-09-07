---
title: "Classe NoPrinterInstalledException"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.NoPrinterInstalledException. Rappresenta un'eccezione che viene sollevata quando non è presente alcuna stampante installata nel sistema operativo"
type: docs
weight: 1100
url: /it/net/aspose.tasks/noprinterinstalledexception/
---
## NoPrinterInstalledException class

Rappresenta un'eccezione che viene lanciata quando non è presente alcuna stampante installata nel sistema operativo.

```csharp
public class NoPrinterInstalledException : Exception
```

## Esempi

Mostra come utilizzare le opzioni di stampa.

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

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


