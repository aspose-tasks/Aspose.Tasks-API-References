---
title: "Prj.EarnedValueMethod"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Prj. El método predeterminado para calcular el valor ganado"
type: docs
weight: 310
url: /es/net/aspose.tasks/prj/earnedvaluemethod/
---
## Prj.EarnedValueMethod field

El método predeterminado para calcular el valor ganado.

```csharp
public static readonly Key<EarnedValueMethodType, PrjKey> EarnedValueMethod;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Prj.EarnedValueMethod.

```csharp
var project = new Project();

project.Set(Prj.EarnedValueMethod, EarnedValueMethodType.PhysicalPercentComplete);

Console.WriteLine("Earned Value Method: " + project.Get(Prj.EarnedValueMethod));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [EarnedValueMethodType](../../earnedvaluemethodtype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


