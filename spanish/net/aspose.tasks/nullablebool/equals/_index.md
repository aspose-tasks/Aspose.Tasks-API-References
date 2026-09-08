---
title: "NullableBool.Equals"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método NullableBool. Devuelve una bandera que indica si esta instancia es igual a la instancia especificada de la clase NullableBool"
type: docs
weight: 40
url: /es/net/aspose.tasks/nullablebool/equals/
---
## Equals(NullableBool) {#equals}

Devuelve una bandera que indica si esta instancia es igual a la instancia especificada de la clase [`NullableBool`](../).

```csharp
public bool Equals(NullableBool other)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| otro | NullableBool | el objeto especificado para comparar con esta instancia. |

### Valor devuelto

una bandera que indica si esta instancia es igual a la instancia especificada de la clase [`NullableBool`](../).

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

## Equals(object) {#equals_1}

Devuelve una bandera que indica si esta instancia es igual al objeto especificado.

```csharp
public override bool Equals(object obj)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | Objeto | el objeto especificado para comparar con esta instancia. |

### Valor devuelto

una bandera que indica si esta instancia es igual al objeto especificado.

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


