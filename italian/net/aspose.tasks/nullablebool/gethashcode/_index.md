---
title: "NullableBool.GetHashCode"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo NullableBool. Restituisce un valore di hash code per l'istanza della classe NullableBool"
type: docs
weight: 50
url: /it/net/aspose.tasks/nullablebool/gethashcode/
---
## NullableBool.GetHashCode method

Restituisce un valore di hash code per l'istanza della classe [`NullableBool`](../).

```csharp
public override int GetHashCode()
```

### Valore di ritorno

restituisce un valore di hash per questo oggetto.

## Esempi

Mostra come lavorare con il metodo &lt;see cref=\"Aspose.Tasks.NullableBool\" /&gt;.GetHashCode.

```csharp
var bool1 = new NullableBool(true);
var bool2 = new NullableBool(true, false);

// l'hash code dei bool è basato sulle proprietà 'IsDefined' e 'Value'
Console.WriteLine("Bool 1: {0} Hash Code 1: {1}", bool1.ToString(), bool1.GetHashCode());
Console.WriteLine("Bool 2: {0} Hash Code 1: {1}", bool2.ToString(), bool2.GetHashCode());
```

### Vedi anche

* struct [NullableBool](../)
* namespace [Aspose.Tasks](../../nullablebool/)
* assembly [Aspose.Tasks](../../../)


