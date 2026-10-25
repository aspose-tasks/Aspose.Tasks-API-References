---
title: "Duration.ParseTimeSpan"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método Duration. Analiza la cadena de duración en formato PTHMS."
type: docs
weight: 130
url: /es/net/aspose.tasks/duration/parsetimespan/
---
## Duration.ParseTimeSpan method

Analiza la cadena de duración en el formato "PT--H--M--S--".

```csharp
public static TimeSpan ParseTimeSpan(string value)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| value | Cadena | la cadena especificada para analizar. |

### Valor devuelto

devuelve una instancia analizada de la estructura [`TimeSpan`](../timespan/).

## Ejemplos

Muestra cómo convertir una cadena en un intervalo de tiempo.

```csharp
var timeSpan = Duration.ParseTimeSpan("PT1H10M30S");
Console.WriteLine("The parsed time span: " + timeSpan);
```

### Ver también

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


