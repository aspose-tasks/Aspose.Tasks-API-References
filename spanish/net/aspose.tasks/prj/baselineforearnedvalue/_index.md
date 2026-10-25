---
title: "Prj.BaselineForEarnedValue"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Campo Prj. La línea base específica utilizada para calcular los valores de variación"
type: docs
weight: 80
url: /es/net/aspose.tasks/prj/baselineforearnedvalue/
---
## Prj.BaselineForEarnedValue field

La línea base específica utilizada para calcular los valores de variación.

```csharp
public static readonly Key<BaselineType, PrjKey> BaselineForEarnedValue;
```

## Ejemplos

Muestra cómo leer/escribir la propiedad Prj.BaselineForEarnedValue.

```csharp
var project = new Project();

project.Set(Prj.BaselineForEarnedValue, BaselineType.Baseline);

Console.WriteLine("Baseline For Earned Value: " + project.Get(Prj.BaselineForEarnedValue));
```

### Ver también

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [BaselineType](../../baselinetype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


