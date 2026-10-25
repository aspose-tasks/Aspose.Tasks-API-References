---
title: "NullableBool.IsDefined"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà NullableBool. Ottiene un valore che indica se il valore era definito, altrimenti false"
type: docs
weight: 20
url: /it/net/aspose.tasks/nullablebool/isdefined/
---
## NullableBool.IsDefined property

Restituisce un valore che indica se il valore è stato definito; altrimenti, false.

```csharp
public bool IsDefined { get; }
```

## Esempi

Mostra come lavorare con la classe &lt;see cref="NullableBool" /&gt;.

```csharp
var project = new Project();

// vediamo dove viene usata la classe <see cref="Aspose.Tasks.NullableBool" />
// Il principale vantaggio di <see cref="Aspose.Tasks.NullableBool" /> è che 
// si può impostare come non definito tramite la costruzione
var actualsInSync = new NullableBool(false, false);
Console.WriteLine("'ActualsInSync' Value: " + actualsInSync.Value);
Console.WriteLine("'ActualsInSync' Is Defined: " + actualsInSync.IsDefined);

// ...
// usa un'istanza di nullable bool
project.Set(Prj.ActualsInSync, actualsInSync);

// ...
var honorConstraints = new NullableBool(true);
Console.WriteLine("'HonorConstraints' ToString: " + honorConstraints.ToString());

// ...
// usa un'istanza di nullable bool
project.Set(Prj.HonorConstraints, honorConstraints);

// ...
```

### Vedi anche

* struct [NullableBool](../)
* namespace [Aspose.Tasks](../../nullablebool/)
* assembly [Aspose.Tasks](../../../)


