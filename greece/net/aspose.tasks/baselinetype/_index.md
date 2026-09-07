---
title: "Απαρίθμηση BaselineType"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Η απαρίθμηση Aspose.Tasks.BaselineType. Καθορίζει τον τύπο βάσης που χρησιμοποιείται για τον υπολογισμό των τιμών Απόκλισης."
type: docs
weight: 130
url: /el/net/aspose.tasks/baselinetype/
---
## BaselineType enumeration

Καθορίζει τον τύπο βάσης που χρησιμοποιείται για τον υπολογισμό των τιμών Απόκλισης.

```csharp
public enum BaselineType
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| Undefined | `-1` | Δείχνει ότι το πεδίο δεν ορίστηκε στο αρχικό αρχείο έργου. |
| Baseline | `0` | Δείχνει τον τύπο Baseline. |
| Baseline1 | `1` | Δείχνει τον τύπο Baseline1. |
| Baseline2 | `2` | Δείχνει τον τύπο Baseline2. |
| Baseline3 | `3` | Δείχνει τον τύπο Baseline3. |
| Baseline4 | `4` | Δείχνει τον τύπο Baseline4. |
| Baseline5 | `5` | Δείχνει τον τύπο Baseline5. |
| Baseline6 | `6` | Δείχνει τον τύπο Baseline6. |
| Baseline7 | `7` | Δείχνει τον τύπο Baseline7. |
| Baseline8 | `8` | Δείχνει τον τύπο Baseline8. |
| Baseline9 | `9` | Δείχνει τον τύπο Baseline9. |
| Baseline10 | `10` | Δείχνει τον τύπο Baseline10. |

## Παρατηρήσεις

Κατά την εξαγωγή σε XML, οι μη ορισμένες τιμές θα αφαιρεθούν από το τελικό XML.

## Παραδείγματα

Δείχνει πώς να ορίσει τη βάση για το έργο (BaselineType.Baseline).

```csharp
var project = new Project(DataDir + "Project2.mpp");
// Αποθηκεύει τα πεδία βάσης στην καθορισμένη βάση για ολόκληρο το έργο.
project.SetBaseline(BaselineType.Baseline);
// εργασία με τις βάσεις του έργου...
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


