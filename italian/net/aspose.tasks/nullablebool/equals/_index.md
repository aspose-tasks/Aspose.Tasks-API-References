---
title: "NullableBool.Equals"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo NullableBool. Restituisce un flag che indica se questa istanza è uguale all'istanza specificata della classe NullableBool"
type: docs
weight: 40
url: /it/net/aspose.tasks/nullablebool/equals/
---
## Equals(NullableBool) {#equals}

Restituisce un flag che indica se questa istanza è uguale all'istanza specificata della classe [`NullableBool`](../).

```csharp
public bool Equals(NullableBool other)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| altro | NullableBool | l'oggetto specificato da confrontare con questa istanza. |

### Valore di ritorno

un flag che indica se questa istanza è uguale all'istanza specificata della classe [`NullableBool`](../).

## Esempi

Mostra come confrontare le istanze di &lt;see cref=\"Aspose.Tasks.NullableBool\" /&gt;.

```csharp
var bool1 = new NullableBool(true);
var bool2 = new NullableBool(true, false);

// L'uguaglianza dei bool viene verificata rispetto alle proprietà 'IsDefined' e 'Value'.
Console.WriteLine("Nullable Bool 1: " + bool1.ToString());
Console.WriteLine("Nullable Bool 2: " + bool2.ToString());

// verifica la conversione implicita a bool: bool1 è True perché è definito e Value è impostato a True.
if (bool1)
{
    Console.WriteLine("Nullable Bool 1 is True");
}
else
{
    Console.WriteLine("Nullable Bool 1 is False");
}

// verifica la conversione implicita a bool: bool2 è False perché non è definito.
if (bool2)
{
    Console.WriteLine("Nullable Bool 2 is True");
}
else
{
    Console.WriteLine("Nullable Bool 2 is False");
}

Console.WriteLine("Are bools equal: " + bool1.Equals(bool2));

// verifica la conversione implicita a bool
if (bool2)
{
    Console.WriteLine("Nullable Bool 2 is True");
}
else
{
    Console.WriteLine("Nullable Bool 2 is False");
}
```

### Vedi anche

* struct [NullableBool](../)
* namespace [Aspose.Tasks](../../nullablebool/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Restituisce una flag che indica se questa istanza è uguale all'oggetto specificato.

```csharp
public override bool Equals(object obj)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | Oggetto | l'oggetto specificato da confrontare con questa istanza. |

### Valore di ritorno

un flag che indica se questa istanza è uguale all'oggetto specificato.

## Esempi

Mostra come confrontare le istanze di &lt;see cref=\"Aspose.Tasks.NullableBool\" /&gt;.

```csharp
var bool1 = new NullableBool(true);
var bool2 = new NullableBool(true, false);

// L'uguaglianza dei bool viene verificata rispetto alle proprietà 'IsDefined' e 'Value'.
Console.WriteLine("Nullable Bool 1: " + bool1.ToString());
Console.WriteLine("Nullable Bool 2: " + bool2.ToString());

// verifica la conversione implicita a bool: bool1 è True perché è definito e Value è impostato a True.
if (bool1)
{
    Console.WriteLine("Nullable Bool 1 is True");
}
else
{
    Console.WriteLine("Nullable Bool 1 is False");
}

// verifica la conversione implicita a bool: bool2 è False perché non è definito.
if (bool2)
{
    Console.WriteLine("Nullable Bool 2 is True");
}
else
{
    Console.WriteLine("Nullable Bool 2 is False");
}

Console.WriteLine("Are bools equal: " + bool1.Equals(bool2));

// verifica la conversione implicita a bool
if (bool2)
{
    Console.WriteLine("Nullable Bool 2 is True");
}
else
{
    Console.WriteLine("Nullable Bool 2 is False");
}
```

### Vedi anche

* struct [NullableBool](../)
* namespace [Aspose.Tasks](../../nullablebool/)
* assembly [Aspose.Tasks](../../../)


