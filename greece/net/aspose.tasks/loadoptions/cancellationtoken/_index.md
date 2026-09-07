---
title: "LoadOptions.CancellationToken"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα LoadOptions. Λαμβάνει ή ορίζει ένα token που μπορεί να χρησιμοποιηθεί για την ακύρωση μιας λειτουργίας φόρτωσης έργου."
type: docs
weight: 20
url: /el/net/aspose.tasks/loadoptions/cancellationtoken/
---
## LoadOptions.CancellationToken property

Λαμβάνει ή ορίζει ένα διακριτικό που μπορεί να χρησιμοποιηθεί για την ακύρωση μιας λειτουργίας φόρτωσης έργου.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Παραδείγματα

Δείχνει πώς να περάσετε το CancellationToken για να ακυρώσετε μια μακρά λειτουργία φόρτωσης έργου.

```csharp
var loadOptions = new LoadOptions();

CancellationTokenSource cts = new CancellationTokenSource();
loadOptions.CancellationToken = cts.Token;

// Το cts μπορεί να περαστεί σε άλλο νήμα όπου η μέθοδος cts.Cancel() μπορεί να κληθεί για να ακυρώσει τη λειτουργία φόρτωσης έργου.
// cts.Cancel();
var project = new Project(DataDir + "PrimaveraProject.xml", loadOptions);
```

### Δείτε επίσης

* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


