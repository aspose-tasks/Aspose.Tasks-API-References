---
title: "Rsc.Phonetics"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Rsc. Η φωνητική γραφή του ονόματος του πόρου. Για χρήση μόνο με Ιαπωνικά"
type: docs
weight: 560
url: /el/net/aspose.tasks/rsc/phonetics/
---
## Rsc.Phonetics field

Η φωνητική γραφή του ονόματος του πόρου. Για χρήση μόνο με Ιαπωνικά.

```csharp
public static readonly Key<string, RscKey> Phonetics;
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε/γράψετε την ιδιότητα Rsc.Phonetics.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Phonetics, "Phonetics");

Console.WriteLine("Phonetics: " + resource.Get(Rsc.Phonetics));
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


