---
title: "Κλάση NoPrinterInstalledException"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κλάση Aspose.Tasks.NoPrinterInstalledException. Αντιπροσωπεύει μια εξαίρεση που ρίχνεται όταν δεν υπάρχει εγκατεστημένος εκτυπωτής στο λειτουργικό σύστημα."
type: docs
weight: 1100
url: /el/net/aspose.tasks/noprinterinstalledexception/
---
## NoPrinterInstalledException class

Αντιπροσωπεύει μια εξαίρεση που ρίχνεται όταν δεν υπάρχει εγκατεστημένος εκτυπωτής στο λειτουργικό σύστημα.

```csharp
public class NoPrinterInstalledException : Exception
```

## Παραδείγματα

Δείχνει πώς να χρησιμοποιήσετε τις επιλογές εκτύπωσης.

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

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


