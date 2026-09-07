---
title: "Duration.ParseTimeSpan"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Duration. Αναλύει τη συμβολοσειρά διάρκειας σε μορφή PTHMS"
type: docs
weight: 130
url: /el/net/aspose.tasks/duration/parsetimespan/
---
## Duration.ParseTimeSpan method

Αναλύει το κείμενο διάρκειας στη μορφή "PT--H--M--S--".

```csharp
public static TimeSpan ParseTimeSpan(string value)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| value | String | τη συγκεκριμένη συμβολοσειρά για ανάλυση. |

### Τιμή Επιστροφής

επιστρέφει την αναλυμένη παρουσία του [`TimeSpan`](../timespan/) struct.

## Παραδείγματα

Δείχνει πώς να μετατρέψετε μια συμβολοσειρά σε ένα χρονικό διάστημα.

```csharp
var timeSpan = Duration.ParseTimeSpan("PT1H10M30S");
Console.WriteLine("The parsed time span: " + timeSpan);
```

### Δείτε επίσης

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


