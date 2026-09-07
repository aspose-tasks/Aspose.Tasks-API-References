---
title: "CopyToOptions.CopyToOptions"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κατασκευαστής CopyToOptions. Αρχικοποιεί μια νέα παρουσία της κλάσης CopyToOptions"
type: docs
weight: 10
url: /el/net/aspose.tasks/copytooptions/copytooptions/
---
## CopyToOptions constructor

Αρχικοποιεί μια νέα παρουσία της κλάσης [`CopyToOptions`](../).

```csharp
public CopyToOptions()
```

## Παραδείγματα

Δείχνει πώς να χρησιμοποιήσετε τις επιλογές αντιγραφής έργου.

```csharp
var project = new Project(DataDir + "CopyToProjectEmpty.xml");
File.Copy(DataDir + "CopyToProjectEmpty.mpp", OutDir + "ProjectCopying_out.mpp", true);

var mppProject = new Project(OutDir + "ProjectCopying_out.mpp");

// παραλείψτε την αντιγραφή των δεδομένων προβολής κατά την αντιγραφή κοινών δεδομένων έργου.
var copyToOptions = new CopyToOptions();
copyToOptions.CopyViewData = false;
project.CopyTo(mppProject, copyToOptions);
```

### Δείτε επίσης

* class [CopyToOptions](../)
* namespace [Aspose.Tasks](../../copytooptions/)
* assembly [Aspose.Tasks](../../../)


