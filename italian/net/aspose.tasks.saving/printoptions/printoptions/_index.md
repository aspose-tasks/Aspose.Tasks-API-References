---
title: "PrintOptions.PrintOptions"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Costruttore di PrintOptions. Inizializza una nuova istanza della classe PrintOptions che può essere usata per impostare diverse opzioni di stampa del progetto"
type: docs
weight: 10
url: /it/net/aspose.tasks.saving/printoptions/printoptions/
---
## PrintOptions constructor

Inizializza una nuova istanza della classe [`PrintOptions`](../) che può essere usata per impostare diverse opzioni di stampa del progetto.

```csharp
public PrintOptions()
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

* class [PrintOptions](../)
* namespace [Aspose.Tasks.Saving](../../printoptions/)
* assembly [Aspose.Tasks](../../../)


