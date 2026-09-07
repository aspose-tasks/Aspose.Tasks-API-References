---
title: "Rsc.Phonetics"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. La trascrizione fonetica del nome della risorsa. Solo per uso con il giapponese"
type: docs
weight: 560
url: /it/net/aspose.tasks/rsc/phonetics/
---
## Rsc.Phonetics field

L'ortografia fonetica del nome della risorsa. Solo per uso con il giapponese.

```csharp
public static readonly Key<string, RscKey> Phonetics;
```

## Esempi

Mostra come leggere/scrivere la proprietà Rsc.Phonetics.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Phonetics, "Phonetics");

Console.WriteLine("Phonetics: " + resource.Get(Rsc.Phonetics));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


