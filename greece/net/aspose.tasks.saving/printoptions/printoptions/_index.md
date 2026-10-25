---
title: "PrintOptions.PrintOptions"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κατασκευαστής PrintOptions. Αρχικοποιεί μια νέα παρουσία της κλάσης PrintOptions που μπορεί να χρησιμοποιηθεί για τον καθορισμό διαφορετικών επιλογών εκτύπωσης του έργου."
type: docs
weight: 10
url: /el/net/aspose.tasks.saving/printoptions/printoptions/
---
## PrintOptions constructor

Αρχικοποιεί μια νέα παρουσία της κλάσης [`PrintOptions`](../) που μπορεί να χρησιμοποιηθεί για τον καθορισμό διαφορετικών επιλογών εκτύπωσης του έργου.

```csharp
public PrintOptions()
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

* class [PrintOptions](../)
* namespace [Aspose.Tasks.Saving](../../printoptions/)
* assembly [Aspose.Tasks](../../../)


