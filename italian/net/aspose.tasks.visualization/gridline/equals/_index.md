---
title: "Gridline.Equals"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo Gridline. Restituisce un valore che indica se questa istanza è uguale all'oggetto specificato"
type: docs
weight: 50
url: /it/net/aspose.tasks.visualization/gridline/equals/
---
## Gridline.Equals method

Restituisce una flag che indica se questa istanza è uguale all'oggetto specificato.

```csharp
public override bool Equals(object obj)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | Oggetto | l'oggetto specificato da confrontare con questa istanza. |

### Valore di ritorno

un flag che indica se questa istanza è uguale all'oggetto specificato.

## Esempi

Mostra come verificare l'uguaglianza delle linee di griglia.

```csharp
var gridline1 = new Gridline();
var gridline2 = new Gridline();

// L'uguaglianza delle linee di griglia è verificata rispetto al tipo di linea di griglia.
Console.WriteLine("Gridline 1 Type: " + gridline1.GridlineType);
Console.WriteLine("Gridline 2 Type: " + gridline2.GridlineType);
Console.WriteLine("Are gridlines equal: " + gridline1.Equals(gridline2));

// cambia il tipo
gridline1.GridlineType = GridlineType.BarRows;
Console.WriteLine("Gridline 1 Type: " + gridline1.GridlineType);
Console.WriteLine("Are gridlines equal: " + gridline1.Equals(gridline2));
```

### Vedi anche

* class [Gridline](../)
* namespace [Aspose.Tasks.Visualization](../../gridline/)
* assembly [Aspose.Tasks](../../../)


