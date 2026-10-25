---
title: "NullableBool.NullableBool"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Costruttore NullableBool. Inizializza una nuova istanza della struct NullableBool con il valore booleano specificato."
type: docs
weight: 10
url: /it/net/aspose.tasks/nullablebool/nullablebool/
---
## NullableBool(bool) {#constructor}

Inizializza una nuova istanza della struct [`NullableBool`](../) con il valore booleano specificato.

```csharp
public NullableBool(bool value)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | Boolean | il valore booleano specificato. |

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

---

## NullableBool(bool, bool) {#constructor_1}

Inizializza una nuova istanza della struttura [`NullableBool`](../).

```csharp
public NullableBool(bool value, bool isDefined)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | Boolean | Il valore corrente. |
| isDefined | Boolean | Il valore che indica se il valore corrente è definito. |

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


