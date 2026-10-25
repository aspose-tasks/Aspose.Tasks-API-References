---
title: "Rsc.IsEnterprise"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Rsc. Indica se una risorsa proviene dal pool di risorse aziendale (true) o dal pool di risorse locale (false)"
type: docs
weight: 400
url: /it/net/aspose.tasks/rsc/isenterprise/
---
## Rsc.IsEnterprise field

Mostra se una risorsa proviene dal pool di risorse aziendale (true) o dal pool di risorse locale (false).

```csharp
public static readonly Key<NullableBool, RscKey> IsEnterprise;
```

## Esempi

Mostra come leggere/scrivere la proprietà Rsc.IsEnterprise.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.IsEnterprise, true);

Console.WriteLine("Is Enterprise: " + resource.Get(Rsc.IsEnterprise));
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


