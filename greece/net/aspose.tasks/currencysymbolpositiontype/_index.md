---
title: "Απαρίθμηση CurrencySymbolPositionType"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.CurrencySymbolPositionType απαρίθμηση. Καθορίζει τη θέση ενός συμβόλου νομίσματος."
type: docs
weight: 370
url: /el/net/aspose.tasks/currencysymbolpositiontype/
---
## CurrencySymbolPositionType enumeration

Καθορίζει τη θέση του συμβόλου νομίσματος.

```csharp
public enum CurrencySymbolPositionType
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| Undefined | `-1` | Δηλώνει ότι η μη ορισμένη τιμή σημαίνει ότι το πεδίο δεν ήταν ορισμένο στο αρχικό αρχείο έργου. |
| Before | `0` | Δείχνει τον τύπο θέσης του συμβόλου νομίσματος Πριν. |
| After | `1` | Δείχνει τον τύπο θέσης του συμβόλου νομίσματος Μετά. |
| BeforeWithSpace | `2` | Δείχνει τον τύπο θέσης του συμβόλου νομίσματος ΠρινΜεΔιάστημα. |
| AfterWithSpace | `3` | Δείχνει τον τύπο θέσης του συμβόλου νομίσματος ΜετάΜεΔιάστημα. |

## Παρατηρήσεις

Κατά την εξαγωγή σε XML, οι μη ορισμένες τιμές θα αφαιρεθούν από το τελικό XML.

## Παραδείγματα

Δείχνει πώς να καθορίσετε τη θέση του συμβόλου νομίσματος (CurrencySymbolPositionType.Before).

```csharp
var project = new Project(DataDir + "Project2.mpp");
// ορίστε τη θέση του συμβόλου νομίσματος
// Πριν, χωρίς διάστημα ($0).
project.Set(Prj.CurrencySymbolPosition, CurrencySymbolPositionType.Before);
// εργαστείτε με το έργο...
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


