---
title: "Enum FileFormat"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.FileFormat enum. Καθορίζει τη μορφή αρχείου των έργων."
type: docs
weight: 590
url: /el/net/aspose.tasks/fileformat/
---
## FileFormat enumeration

Καθορίζει τη μορφή αρχείου του έργου.

```csharp
public enum FileFormat
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| Undefined | `0` | Δεν μπορεί να οριστεί. |
| P6XML | `1` | Αναπαριστά τη μορφή Primavera P6 XML. |
| XML | `2` | Μορφή Microsoft Project XML. |
| MPP8 | `3` | Μορφή Microsoft Project 2000. |
| MPP9 | `4` | Μορφή Microsoft Project 2003. |
| MPP12 | `5` | Μορφή Microsoft Project 2007. |
| MPP14 | `6` | Μορφή Microsoft Project 2010. |
| MPT9 | `7` | Μορφή προτύπου Microsoft Project 2003. |
| MPT12 | `8` | Μορφή προτύπου Microsoft Project 2007. |
| MPT14 | `9` | Μορφή προτύπου Microsoft Project 2010 (2013). |
| MPX | `10` | Μορφή αρχείου Mpx |
| XER | `11` | Αναπαριστά τη μορφή Primavera XER |
| HTML | `12` | Αναπαριστά τη μορφή HTML |
| ProjectServer | `13` | Το έργο διαβάστηκε από το Project Server ή το Project Online |

## Παραδείγματα

Δείχνει πώς να διαβάσετε τη μορφή αρχείου ελέγχου έργου.

```csharp
var info = Project.GetProjectFileInfo(DataDir + "Project.xml");
Console.WriteLine("CanRead: " + info.CanRead);
Console.WriteLine("ProjectApplicationInfo: " + info.ProjectApplicationInfo);
Console.WriteLine("ProjectFileFormat: " + info.ProjectFileFormat);
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


