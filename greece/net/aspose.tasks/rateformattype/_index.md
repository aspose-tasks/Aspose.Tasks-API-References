---
title: "Απαρίθμηση RateFormatType"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Απαρίθμηση Aspose.Tasks.RateFormatType. Καθορίζει τις μονάδες που χρησιμοποιεί το Microsoft Project για την εμφάνιση ενός ρυθμού."
type: docs
weight: 1640
url: /el/net/aspose.tasks/rateformattype/
---
## RateFormatType enumeration

Καθορίζει τις μονάδες που χρησιμοποιεί το Microsoft Project για την εμφάνιση ενός ρυθμού.

```csharp
public enum RateFormatType
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| Undefined | `-1` | Η τιμή δεν ορίστηκε στο αρχικό αρχείο έργου. |
| Minute | `0` | Λεπτό ("min") |
| Hour | `1` | Ώρα ("hr") |
| Day | `2` | Ημέρα ("day") |
| Week | `3` | Εβδομάδα ("wk") |
| Month | `4` | Μήνας ("mo") |
| Year | `5` | Έτος ("yr") |
| MaterialResourceRate | `6` | Τιμή υλικού πόρου (κενό) |

## Παρατηρήσεις

Κατά την εξαγωγή σε XML, οι μη ορισμένες τιμές θα αφαιρεθούν από το τελικό XML.

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Rsc.StandardRateFormat.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.StandardRateFormat, RateFormatType.Hour);

Console.WriteLine("Standard Rate Format: " + resource.Get(Rsc.StandardRateFormat));
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


