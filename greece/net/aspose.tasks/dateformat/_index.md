---
title: "Απαρίθμηση DateFormat"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Η απαρίθμηση Aspose.Tasks.DateFormat. Καθορίζει τη μορφή ημερομηνίας."
type: docs
weight: 430
url: /el/net/aspose.tasks/dateformat/
---
## DateFormat enumeration

Καθορίζει τη μορφή ημερομηνίας.

```csharp
public enum DateFormat
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| DateMmDdYyHhMmAM | `0` | Το παράδειγμα: 09/30/02 13:00 μμ. |
| DateMmDdYy | `1` | Το παράδειγμα: 9/30/02 |
| DateMmmmDdYyyyHhMmAM | `2` | Το παράδειγμα: Σεπτέμβριος 30, 2002 13:00 μμ. |
| DateMmmmDdYyyy | `3` | Το παράδειγμα: Σεπτέμβριος 30, 2002 |
| DateMmmDdHhMmAM | `4` | Το παράδειγμα: Σεπ 30 13:00 μμ. |
| DateMmmDdYyy | `5` | Το παράδειγμα: Sep 30, '02 |
| DateMmmmDd | `6` | Το παράδειγμα: Σεπτέμβριος 30 |
| DateMmmDd | `7` | Το παράδειγμα: Sep 30 |
| DateDddMmDdYyHhMmAM | `8` | Το παράδειγμα: Tue 9/30/02 13:00 PM |
| DateDddMmDdYy | `9` | Το παράδειγμα: Tue 9/30/02 |
| DateDddMmmDdYyy | `10` | Το παράδειγμα: Tue Sep 30, '02 |
| DateDddHhMmAM | `11` | Το παράδειγμα: Tue 13:00 PM |
| DateMmDd | `12` | Το παράδειγμα: 9/30 |
| DateDd | `13` | Το παράδειγμα: 30 |
| DateHhMmAm | `14` | Το παράδειγμα: 13:00 PM |
| DateDddMmmDd | `15` | Το παράδειγμα: Tue Sep 30 |
| DateDddMmDd | `16` | Το παράδειγμα: Tue 9/30 |
| DateDddDd | `17` | Το παράδειγμα: Tue 30 |
| DateWwwDd | `18` | Το παράδειγμα: W41/2 |
| DateWwwDdYyHhMmAm | `19` | Το παράδειγμα: W41/2/02 13:00 PM |
| DateMmDdYyyy | `20` | Το παράδειγμα: 9/30/2002 |
| Custom | `21` | Οι τιμές DateTime μορφοποιούνται χρησιμοποιώντας τη συμβολοσειρά μορφής που ορίζεται στην ιδιότητα [`CustomDateFormat`](../prj/customdateformat/) του έργου. |
| DateDdMmYyyy | `256` | Το παράδειγμα: 19/07/2016 |
| Default | `255` | Το παράδειγμα: Προεπιλεγμένη μορφή ημερομηνίας. |

## Παραδείγματα

Δείχνει πώς να προσαρμόσετε τη μορφή ημερομηνίας όλων των ημερομηνιών στο έργο για εξαγωγή.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
project.Set(Prj.StartDate, new DateTime(2014, 9, 22));

// Από προεπιλογή project.DateFormat == DateFormat.Date_ddd_mm_dd_yy (Mon 09/22/14) προσαρμόστε το DateFormat (September 22, 2014)
project.Set(Prj.DateFormat, DateFormat.DateMmmmDdYyyy);
project.Save(OutDir + "CustomizeDateFormats1_out.pdf", SaveFileFormat.Pdf);

// Εξαγωγή σε μορφή ημερομηνίας 19/07/2016
project.Set(Prj.DateFormat, DateFormat.DateDdMmYyyy);
project.Save(OutDir + "CustomizeDateFormats2_out.pdf", SaveFileFormat.Pdf);
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


