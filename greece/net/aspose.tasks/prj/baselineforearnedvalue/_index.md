---
title: "Prj.BaselineForEarnedValue"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Prj πεδίο. Η συγκεκριμένη βασική γραμμή που χρησιμοποιείται για τον υπολογισμό τιμών απόκλισης"
type: docs
weight: 80
url: /el/net/aspose.tasks/prj/baselineforearnedvalue/
---
## Prj.BaselineForEarnedValue field

Η συγκεκριμένη γραμμή βάσης που χρησιμοποιείται για τον υπολογισμό των τιμών Απόκλισης.

```csharp
public static readonly Key<BaselineType, PrjKey> BaselineForEarnedValue;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Prj.BaselineForEarnedValue.

```csharp
var project = new Project();

project.Set(Prj.BaselineForEarnedValue, BaselineType.Baseline);

Console.WriteLine("Baseline For Earned Value: " + project.Get(Prj.BaselineForEarnedValue));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [BaselineType](../../baselinetype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


