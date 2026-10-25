---
title: "NullableBool.op_Equality"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo NullableBool. Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato"
type: docs
weight: 70
url: /it/net/aspose.tasks/nullablebool/op_equality/
---
## NullableBool Equality operator

Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato.

```csharp
public static bool operator ==(NullableBool a, NullableBool b)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| a | NullableBool | Il primo [`NullableBool`](../). |
| b | NullableBool | Il secondo [`NullableBool`](../). |

### Valore di ritorno

un valore che indica se questa istanza è uguale a un oggetto specificato

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


