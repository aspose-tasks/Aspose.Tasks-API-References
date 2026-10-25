---
title: "NullableBool.GetHashCode"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método NullableBool. Devuelve un valor de código hash para la instancia de la clase NullableBool"
type: docs
weight: 50
url: /es/net/aspose.tasks/nullablebool/gethashcode/
---
## NullableBool.GetHashCode method

Devuelve un valor de código hash para la instancia de la clase [`NullableBool`](../).

```csharp
public override int GetHashCode()
```

### Valor devuelto

devuelve un valor de código hash para este objeto.

## Ejemplos

Muestra cómo trabajar con el método &lt;see cref="Aspose.Tasks.NullableBool" /&gt;.GetHashCode.

```csharp
var bool1 = new NullableBool(true);
var bool2 = new NullableBool(true, false);

// el código hash de los booleanos se basa en las propiedades 'IsDefined' y 'Value'
Console.WriteLine("Bool 1: {0} Hash Code 1: {1}", bool1.ToString(), bool1.GetHashCode());
Console.WriteLine("Bool 2: {0} Hash Code 1: {1}", bool2.ToString(), bool2.GetHashCode());
```

### Ver también

* struct [NullableBool](../)
* namespace [Aspose.Tasks](../../nullablebool/)
* assembly [Aspose.Tasks](../../../)


