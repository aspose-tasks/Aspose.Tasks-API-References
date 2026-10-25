---
title: "Klasse NoPrinterInstalledException"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.NoPrinterInstalledException-klasse. Vertegenwoordigt een uitzondering die wordt gegooid wanneer er geen printer is geïnstalleerd in het besturingssysteem"
type: docs
weight: 1100
url: /nl/net/aspose.tasks/noprinterinstalledexception/
---
## NoPrinterInstalledException class

Stelt een uitzondering voor die wordt gegooid wanneer er geen geïnstalleerde printer in het besturingssysteem aanwezig is.

```csharp
public class NoPrinterInstalledException : Exception
```

## Voorbeelden

Toont hoe afdrukopties te gebruiken.

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

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


