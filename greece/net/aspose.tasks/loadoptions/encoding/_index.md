---
title: "LoadOptions.Encoding"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα LoadOptions. Λαμβάνει ή ορίζει την κωδικοποίηση που χρησιμοποιείται για την ανάγνωση ενός έργου από μορφές HTML, MPX, XER και Primavera XML. Η προεπιλεγμένη κωδικοποίηση είναι UTF8."
type: docs
weight: 30
url: /el/net/aspose.tasks/loadoptions/encoding/
---
## LoadOptions.Encoding property

Λαμβάνει ή ορίζει την κωδικοποίηση που χρησιμοποιείται για την ανάγνωση ενός έργου από μορφές HTML, MPX, XER και Primavera XML. Η προεπιλεγμένη κωδικοποίηση είναι UTF8.

```csharp
public Encoding Encoding { get; set; }
```

## Παραδείγματα

Δείχνει πώς να καθορίσετε την κωδικοποίηση κατά το άνοιγμα ενός έργου από αρχείο Primavera XER.

```csharp
LoadOptions lo = new LoadOptions();
lo.Encoding = Encoding.GetEncoding(1251);
lo.PrimaveraReadOptions = new PrimaveraReadOptions();
var project = new Project("encoding1251.xer", lo);
```

### Δείτε επίσης

* class [LoadOptions](../)
* namespace [Aspose.Tasks](../../loadoptions/)
* assembly [Aspose.Tasks](../../../)


