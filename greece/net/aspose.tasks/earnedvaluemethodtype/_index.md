---
title: "Enum EarnedValueMethodType"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Aspose.Tasks.EarnedValueMethodType enum. Καθορίζει τη μέθοδο που χρησιμοποιείται για τον υπολογισμό της κερδισμένης αξίας"
type: docs
weight: 480
url: /el/net/aspose.tasks/earnedvaluemethodtype/
---
## EarnedValueMethodType enumeration

Καθορίζει τη μέθοδο που χρησιμοποιείται για τον υπολογισμό της κερδισμένης αξίας.

```csharp
public enum EarnedValueMethodType
```

### Τιμές

| Όνομα | Τιμή | Περιγραφή |
| --- | --- | --- |
| Undefined | `-1` | Το πεδίο δεν ορίστηκε στο αρχικό αρχείο έργου. |
| PercentComplete | `0` | Ποσοστό ολοκλήρωσης |
| PhysicalPercentComplete | `1` | Φυσικό ποσοστό ολοκλήρωσης |

## Παρατηρήσεις

Κατά την εξαγωγή σε XML, οι μη ορισμένες τιμές θα αφαιρεθούν από το τελικό XML.

## Παραδείγματα

Δείχνει πώς να καθορίσετε τη μέθοδο που χρησιμοποιείται για τον υπολογισμό της κερδισμένης αξίας (EarnedValueMethodType.PercentComplete).

```csharp
var project = new Project(DataDir + "Project2.mpp");
// ορίστε τον τύπο μεθόδου κερδισμένης αξίας σε 'PercentComplete'
project.Set(Prj.DefaultTaskEVMethod, EarnedValueMethodType.PercentComplete);
// εργαστείτε με το έργο...
```

### Δείτε επίσης

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


