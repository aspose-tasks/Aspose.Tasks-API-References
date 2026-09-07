---
title: "Απαρίθμηση ApplicationInfo"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.ApplicationInfo απαρίθμηση. Καθορίζει την έκδοση του έργου όπου δημιουργήθηκε το αρχείο"
type: docs
weight: 10
url: /el/net/aspose.tasks/applicationinfo/
---
## ApplicationInfo enumeration

Καθορίζει την έκδοση του έργου όπου δημιουργήθηκε το αρχείο.

```csharp
public enum ApplicationInfo
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| Undefined | `0` | Δεν μπορεί να οριστεί. |
| MSP2000 | `1` | Το αρχείο δημιουργήθηκε στο Microsoft Project 2000/2002. |
| MSP2003 | `2` | Το αρχείο δημιουργήθηκε στο Microsoft Project 2003. |
| MSP2007 | `3` | Το αρχείο δημιουργήθηκε στο Microsoft Project 2007. |
| MSP2010 | `4` | Το αρχείο δημιουργήθηκε στο Microsoft Project 2010. |
| MSP2013 | `5` | Το αρχείο δημιουργήθηκε στο Microsoft Project 2013. |
| MSP2016 | `6` | Το αρχείο δημιουργήθηκε στο Microsoft Project 2016. |

## Παραδείγματα

Δείχνει πώς να ελέγξετε τις πληροφορίες εφαρμογής του έργου.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


