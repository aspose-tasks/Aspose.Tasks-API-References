---
title: "Prj.MicrosoftProjectServerURL"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Prj. Καθορίζει αν ένα έργο δημιουργήθηκε από χρήστη Project Server σε αντίθεση με χρήστη NT"
type: docs
weight: 460
url: /el/net/aspose.tasks/prj/microsoftprojectserverurl/
---
## Prj.MicrosoftProjectServerURL field

Καθορίζει εάν ένα έργο δημιουργήθηκε από χρήστη Project Server σε αντίθεση με χρήστη NT.

```csharp
public static readonly Key<NullableBool, PrjKey> MicrosoftProjectServerURL;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Prj.MicrosoftProjectServerURL.

```csharp
var project = new Project();

project.Set(Prj.MicrosoftProjectServerURL, true);

Console.WriteLine("Microsoft Project Server U R L: " + project.Get(Prj.MicrosoftProjectServerURL));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


