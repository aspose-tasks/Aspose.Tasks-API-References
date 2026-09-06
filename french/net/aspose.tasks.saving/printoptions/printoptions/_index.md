---
title: "PrintOptions.PrintOptions"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Constructeur PrintOptions. Initialise une nouvelle instance de la classe PrintOptions qui peut être utilisée pour définir différentes options d'impression du projet"
type: docs
weight: 10
url: /fr/net/aspose.tasks.saving/printoptions/printoptions/
---
## PrintOptions constructor

Initialise une nouvelle instance de la classe [`PrintOptions`](../) qui peut être utilisée pour définir différentes options d'impression du projet.

```csharp
public PrintOptions()
```

## Exemples

Montre comment utiliser les options d'impression.

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

### Voir aussi

* class [PrintOptions](../)
* namespace [Aspose.Tasks.Saving](../../printoptions/)
* assembly [Aspose.Tasks](../../../)


