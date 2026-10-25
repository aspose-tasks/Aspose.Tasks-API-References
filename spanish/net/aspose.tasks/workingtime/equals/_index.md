---
title: "WorkingTime.Equals"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método WorkingTime. Verifica que los objetos sean iguales"
type: docs
weight: 40
url: /es/net/aspose.tasks/workingtime/equals/
---
## WorkingTime.Equals method

Comprueba que los objetos son iguales.

```csharp
public override bool Equals(object obj)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| obj | Objeto | Segundo objeto a comparar. |

### Valor devuelto

True si los objetos son iguales, false en caso contrario.

## Ejemplos

Muestra cómo comprobar la igualdad del tiempo de trabajo.

```csharp
var workingTime1 = new WorkingTime(9, 12);
var workingTime2 = new WorkingTime(13, 17);

// La igualdad de los calendarios se verifica contra las fechas de inicio y fin del tiempo de trabajo.
Console.WriteLine("Working Time 1 (From): " + workingTime1.From);
Console.WriteLine("Working Time 1 (To): " + workingTime1.To);

Console.WriteLine("Working Time 2 (From): " + workingTime2.From);
Console.WriteLine("Working Time 2 (To): " + workingTime2.To);
Console.WriteLine("Are working times equal: " + workingTime1.Equals(workingTime2));
```

### Ver también

* class [WorkingTime](../)
* namespace [Aspose.Tasks](../../workingtime/)
* assembly [Aspose.Tasks](../../../)


