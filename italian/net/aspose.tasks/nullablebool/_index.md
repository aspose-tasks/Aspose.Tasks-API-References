---
title: "Struttura NullableBool"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Struct Aspose.Tasks.NullableBool. Una classe per valori booleani con la possibilità di verificare se il valore è stato definito o meno."
type: docs
weight: 1110
url: /it/net/aspose.tasks/nullablebool/
---
## NullableBool structure

Una classe per valori booleani con la possibilità di verificare se il valore è stato definito o meno.

```csharp
public struct NullableBool : IEquatable<NullableBool>
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [NullableBool](nullablebool/#constructor)(bool) | Inizializza una nuova istanza della struct `NullableBool` con il valore booleano specificato. |
| [NullableBool](nullablebool/#constructor_1)(bool, bool) | Inizializza una nuova istanza della struct `NullableBool`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [IsDefined](../../aspose.tasks/nullablebool/isdefined/) { get; } | Restituisce un valore che indica se il valore è stato definito; altrimenti, false. |
| [Value](../../aspose.tasks/nullablebool/value/) { get; set; } | Ottiene o imposta un valore che indica se il valore corrente è true o false. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Equals](../../aspose.tasks/nullablebool/equals/#equals)(NullableBool) | Restituisce un flag che indica se questa istanza è uguale all'istanza specificata della classe `NullableBool`. |
| override [Equals](../../aspose.tasks/nullablebool/equals/#equals_1)(object) | Restituisce una flag che indica se questa istanza è uguale all'oggetto specificato. |
| override [GetHashCode](../../aspose.tasks/nullablebool/gethashcode/)() | Restituisce un valore di hash code per l'istanza della classe `NullableBool`. |
| override [ToString](../../aspose.tasks/nullablebool/tostring/)() | Restituisce una stringa che rappresenta l'oggetto corrente. |
| [operator ==](../../aspose.tasks/nullablebool/op_equality/) | Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato. |
| [implicit operator](../../aspose.tasks/nullablebool/op_implicit/#op_implicit_1) | Converte implicitamente un'istanza di `NullableBool` in un valore booleano. Restituisce true quando [`Value`](./value/) è true e [`IsDefined`](./isdefined/) è true. (2 operatori) |
| [operator !=](../../aspose.tasks/nullablebool/op_inequality/) | Restituisce un valore che indica se questa istanza non è uguale a un oggetto specificato. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


