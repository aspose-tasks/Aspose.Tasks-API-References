---
title: "NullableBool.op_Implicit"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo NullableBool. Converte implicitamente un'istanza NullableBool in un valore booleano. Restituisce true quando Value è true e IsDefined è true."
type: docs
weight: 80
url: /it/net/aspose.tasks/nullablebool/op_implicit/
---
## implicit operator {#op_implicit_1}

Converte implicitamente un'istanza di [`NullableBool`](../) in un valore booleano. Restituisce true quando [`Value`](../value/) è true e [`IsDefined`](../isdefined/) è true.

```csharp
public static implicit operator bool(NullableBool val)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| val | NullableBool | Il valore da convertire. |

### Valore di ritorno

un valore booleano.

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

## implicit operator {#op_implicit}

Converte implicitamente un valore booleano nell'istanza [`NullableBool`](../).

```csharp
public static implicit operator NullableBool(bool val)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| val | Boolean | Valore da convertire. |

### Valore di ritorno

Istanza [`NullableBool`](../) convertita.

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


