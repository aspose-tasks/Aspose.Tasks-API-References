---
title: "MpdSettings.MpdSettings"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Κατασκευαστής MpdSettings. Αρχικοποιεί ένα νέο αντικείμενο της κλάσης MpdSettings."
type: docs
weight: 10
url: /el/net/aspose.tasks.connectivity/mpdsettings/mpdsettings/
---
## MpdSettings constructor

Αρχικοποιεί ένα νέο αντικείμενο της κλάσης [`MpdSettings`](../).

```csharp
public MpdSettings(string connectionString, int projectId)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| connectionString | String | η καθορισμένη συμβολοσειρά σύνδεσης. |
| projectId | Int32 | το καθορισμένο id ενός έργου για ανάγνωση. |

## Παραδείγματα

Δείχνει πώς να διαβάσετε ένα έργο από αρχείο MPD.

```csharp
DbSettings settings = new MpdSettings("Provider=Microsoft.Jet.OLEDB.4.0; Data Source=" + DataDir + "MpdFileToRead.mpd", 1);
var project = new Project(settings);
Console.WriteLine(project.Get(Prj.Name));
```

### Δείτε επίσης

* class [MpdSettings](../)
* namespace [Aspose.Tasks.Connectivity](../../mpdsettings/)
* assembly [Aspose.Tasks](../../../)


