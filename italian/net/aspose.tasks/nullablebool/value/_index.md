---
title: "NullableBool.Value"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà NullableBool. Ottiene o imposta un valore che indica se il valore corrente è vero o falso."
type: docs
weight: 30
url: /it/net/aspose.tasks/nullablebool/value/
---
## NullableBool.Value property

Ottiene o imposta un valore che indica se il valore corrente è true o false.

```csharp
public bool Value { get; set; }
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


