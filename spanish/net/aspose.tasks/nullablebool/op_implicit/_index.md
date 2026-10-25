---
title: "NullableBool.op_Implicit"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método NullableBool. Convierte implícitamente una instancia de NullableBool a un valor booleano. Devuelve verdadero cuando Value es verdadero y IsDefined es verdadero"
type: docs
weight: 80
url: /es/net/aspose.tasks/nullablebool/op_implicit/
---
## implicit operator {#op_implicit_1}

Convierte implícitamente una instancia de [`NullableBool`](../) a un valor booleano. Devuelve verdadero cuando [`Value`](../value/) es verdadero y [`IsDefined`](../isdefined/) es verdadero.

```csharp
public static implicit operator bool(NullableBool val)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | NullableBool | El valor a convertir. |

### Valor devuelto

un valor booleano.

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

---

## implicit operator {#op_implicit}

Convierte implícitamente un valor booleano a la instancia [`NullableBool`](../).

```csharp
public static implicit operator NullableBool(bool val)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | Boolean | Valor a convertir. |

### Valor devuelto

Instancia [`NullableBool`](../) convertida.

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


