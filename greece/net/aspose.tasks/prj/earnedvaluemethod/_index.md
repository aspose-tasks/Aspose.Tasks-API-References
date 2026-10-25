---
title: "Prj.EarnedValueMethod"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Prj. Η προεπιλεγμένη μέθοδος υπολογισμού της κερδισμένης αξίας"
type: docs
weight: 310
url: /el/net/aspose.tasks/prj/earnedvaluemethod/
---
## Prj.EarnedValueMethod field

Η προεπιλεγμένη μέθοδος υπολογισμού της κερδισμένης αξίας.

```csharp
public static readonly Key<EarnedValueMethodType, PrjKey> EarnedValueMethod;
```

## Παραδείγματα

Εμφανίζει πώς να διαβάσετε/γράψετε την ιδιότητα Prj.EarnedValueMethod.

```csharp
var project = new Project();

project.Set(Prj.EarnedValueMethod, EarnedValueMethodType.PhysicalPercentComplete);

Console.WriteLine("Earned Value Method: " + project.Get(Prj.EarnedValueMethod));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [EarnedValueMethodType](../../earnedvaluemethodtype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


