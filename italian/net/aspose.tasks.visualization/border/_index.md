---
title: "Enum Border"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Aspose.Tasks.Visualization.Border enum. Specifica il tipo di bordi."
type: docs
weight: 2970
url: /it/net/aspose.tasks.visualization/border/
---
## Border enumeration

Specifica il tipo di bordi.

```csharp
public enum Border
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| NoBorder | `0` | Nessun bordo. |
| AroundEveryPage | `1` | Intorno a ogni pagina. |
| OutsidePages | `2` | Nelle pagine esterne. |

## Esempi

Mostra come lavorare con i margini di pagina.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// consente di modificare la vista predefinita
var margins = project.DefaultView.PageInfo.Margins;

// consente di modificare i margini
margins.Left = 10d;
margins.Top = 10d;
margins.Right = 10d;
margins.Bottom = 10d;
margins.Borders = Border.OutsidePages;

project.Save(OutDir + "WorkWithPageMargins_out.mpp", SaveFileFormat.Mpp);
```

### Vedi anche

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


