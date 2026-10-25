---
title: "Duration.Parse"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método Duration. Convierte la cadena especificada en la instancia de la estructura Duration"
type: docs
weight: 10
url: /es/net/aspose.tasks/duration/parse/
---
## Duration.Parse method

Convierte la cadena especificada en la instancia de la estructura [`Duration`](../).

```csharp
public static Duration Parse(Project p, string value)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| p | Project | la instancia especificada de la clase [`Project`](../../project/) para la cual convertir la duración. |
| value | Cadena | la cadena especificada para convertir. |

### Valor devuelto

Devuelve la instancia convertida de la estructura [`Duration`](../).

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

* class [Project](../../project/)
* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


