---
title: "NullableBool.op_Inequality"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método NullableBool. Devuelve un valor que indica si esta instancia no es igual a un objeto especificado"
type: docs
weight: 90
url: /es/net/aspose.tasks/nullablebool/op_inequality/
---
## NullableBool Inequality operator

Devuelve un valor que indica si esta instancia no es igual a un objeto especificado.

```csharp
public static bool operator !=(NullableBool a, NullableBool b)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| a | NullableBool | El primero [`NullableBool`](../). |
| b | NullableBool | El segundo [`NullableBool`](../). |

### Valor devuelto

un valor que indica si esta instancia no es igual a un objeto especificado

## Ejemplos

Muestra cómo comparar instancias &lt;see cref=\"Aspose.Tasks.NullableBool\" /&gt;.

```csharp
var bool1 = new NullableBool(true);
var bool2 = new NullableBool(true, false);

// la igualdad de los bool se verifica contra las propiedades 'IsDefined' y 'Value'.
Console.WriteLine("Nullable Bool 1: " + bool1.ToString());
Console.WriteLine("Nullable Bool 2: " + bool2.ToString());

// verifica la conversión implícita a bool: bool1 es Verdadero porque está definido y Value está establecido en Verdadero.
if (bool1)
{
    Console.WriteLine("Nullable Bool 1 is True");
}
else
{
    Console.WriteLine("Nullable Bool 1 is False");
}

// verifica la conversión implícita a bool: bool2 es Falso porque no está definido.
if (bool2)
{
    Console.WriteLine("Nullable Bool 2 is True");
}
else
{
    Console.WriteLine("Nullable Bool 2 is False");
}

Console.WriteLine("Are bools equal: " + bool1.Equals(bool2));

// verifica la conversión implícita a bool
if (bool2)
{
    Console.WriteLine("Nullable Bool 2 is True");
}
else
{
    Console.WriteLine("Nullable Bool 2 is False");
}
```

### Ver también

* struct [NullableBool](../)
* namespace [Aspose.Tasks](../../nullablebool/)
* assembly [Aspose.Tasks](../../../)


