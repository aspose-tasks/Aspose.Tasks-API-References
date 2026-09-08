---
title: "Gridline.Equals"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método Gridline. Devuelve una bandera que indica si esta instancia es igual al objeto especificado."
type: docs
weight: 50
url: /es/net/aspose.tasks.visualization/gridline/equals/
---
## Gridline.Equals method

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

Muestra cómo comprobar la igualdad de líneas de cuadrícula.

```csharp
var gridline1 = new Gridline();
var gridline2 = new Gridline();

// La igualdad de líneas de cuadrícula se verifica contra el tipo de línea de cuadrícula.
Console.WriteLine("Gridline 1 Type: " + gridline1.GridlineType);
Console.WriteLine("Gridline 2 Type: " + gridline2.GridlineType);
Console.WriteLine("Are gridlines equal: " + gridline1.Equals(gridline2));

// cambiar el tipo
gridline1.GridlineType = GridlineType.BarRows;
Console.WriteLine("Gridline 1 Type: " + gridline1.GridlineType);
Console.WriteLine("Are gridlines equal: " + gridline1.Equals(gridline2));
```

### Ver también

* class [Gridline](../)
* namespace [Aspose.Tasks.Visualization](../../gridline/)
* assembly [Aspose.Tasks](../../../)


