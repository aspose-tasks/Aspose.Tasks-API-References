---
title: "NullableBool.op_Inequality"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "NullableBool-methode. Retourneert een waarde die aangeeft of dit exemplaar niet gelijk is aan een opgegeven object"
type: docs
weight: 90
url: /nl/net/aspose.tasks/nullablebool/op_inequality/
---
## NullableBool Inequality operator

Retourneert een waarde die aangeeft of deze instantie niet gelijk is aan een opgegeven object.

```csharp
public static bool operator !=(NullableBool a, NullableBool b)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| a | NullableBool | De eerste [`NullableBool`](../). |
| b | NullableBool | De tweede [`NullableBool`](../). |

### Retourwaarde

een waarde die aangeeft of deze instantie niet gelijk is aan een opgegeven object

## Voorbeelden

Toont hoe &lt;see cref="Aspose.Tasks.NullableBool" /&gt;-instanties te vergelijken.

```csharp
var bool1 = new NullableBool(true);
var bool2 = new NullableBool(true, false);

// De gelijkheid van bools wordt gecontroleerd ten opzichte van de 'IsDefined'- en 'Value'-eigenschappen.
Console.WriteLine("Nullable Bool 1: " + bool1.ToString());
Console.WriteLine("Nullable Bool 2: " + bool2.ToString());

// controleert impliciete conversie naar bool: bool1 is True omdat deze gedefinieerd is en Value op True staat.
if (bool1)
{
    Console.WriteLine("Nullable Bool 1 is True");
}
else
{
    Console.WriteLine("Nullable Bool 1 is False");
}

// controleert impliciete conversie naar bool: bool2 is False omdat deze niet gedefinieerd is.
if (bool2)
{
    Console.WriteLine("Nullable Bool 2 is True");
}
else
{
    Console.WriteLine("Nullable Bool 2 is False");
}

Console.WriteLine("Are bools equal: " + bool1.Equals(bool2));

// controleert impliciete conversie naar bool
if (bool2)
{
    Console.WriteLine("Nullable Bool 2 is True");
}
else
{
    Console.WriteLine("Nullable Bool 2 is False");
}
```

### Zie ook

* struct [NullableBool](../)
* namespace [Aspose.Tasks](../../nullablebool/)
* assembly [Aspose.Tasks](../../../)


