---
title: "PrintOptions.PrintOptions"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "PrintOptions constructor. Initialiseert een nieuw exemplaar van de PrintOptions-klasse die kan worden gebruikt om verschillende opties voor het afdrukken van een project in te stellen"
type: docs
weight: 10
url: /nl/net/aspose.tasks.saving/printoptions/printoptions/
---
## PrintOptions constructor

Initialiseert een nieuw exemplaar van de [`PrintOptions`](../) klasse die kan worden gebruikt om verschillende opties voor het afdrukken van een project in te stellen.

```csharp
public PrintOptions()
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

* class [PrintOptions](../)
* namespace [Aspose.Tasks.Saving](../../printoptions/)
* assembly [Aspose.Tasks](../../../)


