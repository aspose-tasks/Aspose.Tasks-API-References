---
title: "Classe NoPrinterInstalledException"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.NoPrinterInstalledException. Représente une exception qui est levée lorsqu'aucune imprimante n'est installée dans le système d'exploitation."
type: docs
weight: 1100
url: /fr/net/aspose.tasks/noprinterinstalledexception/
---
## NoPrinterInstalledException class

Représente une exception qui est levée lorsqu'aucune imprimante n'est installée dans le système d'exploitation.

```csharp
public class NoPrinterInstalledException : Exception
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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


