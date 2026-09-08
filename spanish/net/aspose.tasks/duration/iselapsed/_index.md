---
title: "Duration.IsElapsed"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad Duration. Obtiene un valor que indica si la unidad de tiempo ha transcurrido. La bandera que determina si esta instancia de Duration ha transcurrido"
type: docs
weight: 20
url: /es/net/aspose.tasks/duration/iselapsed/
---
## Duration.IsElapsed property

Obtiene un valor que indica si la unidad de tiempo está transcurrida. La bandera que determina si esta instancia de Duration está transcurrida.

```csharp
public bool IsElapsed { get; }
```

## Ejemplos

Muestra cómo analizar una cadena a partir de una cadena con formato especial.

```csharp
var project = new Project();

// ejemplos de duraciones:
// "1d", "1dy", "1d?", "1day", "1 dy", "1 edy? ", "8hr", "8 hour", "8hours", "0.2w?", "0.2wk", "0.2 eweek", "0.2ew?"
// donde 1 - número de elementos (día, semana, etc), d - día (h - hora, w - semana) ? - bandera estimada, e - bandera transcurrida

// intentar analizar una duración estimada
var duration1 = Duration.Parse(project, "1d?");
Console.WriteLine("The parsed time span: " + duration1.TimeSpan);
Console.WriteLine("The parsed time unit: " + duration1.TimeUnit);
Console.WriteLine("Is estimated duration?: " + duration1.IsEstimated);
Console.WriteLine("Is elapsed duration?: " + duration1.IsElapsed);
Console.WriteLine();

// intentar analizar una duración estimada
var duration2 = Duration.Parse(project, "0.2 eweek");
Console.WriteLine("The parsed time span: " + duration2.TimeSpan);
Console.WriteLine("The parsed time unit: " + duration2.TimeUnit);
Console.WriteLine("Is estimated duration?: " + duration2.IsEstimated);
Console.WriteLine("Is elapsed duration?: " + duration2.IsElapsed);
```

### Ver también

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


