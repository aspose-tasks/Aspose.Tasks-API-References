---
title: "NullableBool.op_Implicit"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "NullableBool-methode. Converteert impliciet een NullableBool‑instantie naar een booleaanse waarde. Retourneert true wanneer Value true is en IsDefined true is"
type: docs
weight: 80
url: /nl/net/aspose.tasks/nullablebool/op_implicit/
---
## implicit operator {#op_implicit_1}

Converteert impliciet een [`NullableBool`](../)‑instantie naar een booleaanse waarde. Retourneert true wanneer [`Value`](../value/) true is en [`IsDefined`](../isdefined/) true is.

```csharp
public static implicit operator bool(NullableBool val)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | NullableBool | De te converteren waarde. |

### Retourwaarde

een booleaanse waarde.

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

---

## implicit operator {#op_implicit}

Converteert impliciet een booleaanse waarde naar de [`NullableBool`](../)‑instantie.

```csharp
public static implicit operator NullableBool(bool val)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | Boolean | Waarde om te converteren. |

### Retourwaarde

Geconverteerde [`NullableBool`](../)‑instantie.

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


