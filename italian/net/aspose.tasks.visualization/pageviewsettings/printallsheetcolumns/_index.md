---
title: "PageViewSettings.PrintAllSheetColumns"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà PageViewSettings. Ottiene o imposta un valore che indica se stampare tutte le colonne del foglio di una visualizzazione"
type: docs
weight: 40
url: /it/net/aspose.tasks.visualization/pageviewsettings/printallsheetcolumns/
---
## PageViewSettings.PrintAllSheetColumns property

Ottiene o imposta un valore che indica se stampare tutte le colonne del foglio di una visualizzazione.

```csharp
public bool PrintAllSheetColumns { get; set; }
```

## Esempi

Mostra come stampare le note di attività, risorsa e assegnazione su una pagina separata.

```csharp
var project = new Project(DataDir + "Input.mpp");

// imposta il numero delle prime colonne da stampare su tutte le pagine
project.DefaultView.PageInfo.PageViewSettings.FirstColumnsCount = 2;

// imposta un valore che indica se stampare le note.
project.DefaultView.PageInfo.PageViewSettings.PrintNotes = true;

// imposta un valore che indica se adattare la scala temporale alla fine di una pagina durante la stampa.
project.DefaultView.PageInfo.PageViewSettings.FitTimescaleToEndOfPage = true;

// imposta un valore che indica se stampare tutte le colonne del foglio di una visualizzazione
project.DefaultView.PageInfo.PageViewSettings.PrintAllSheetColumns = true;

// imposta un valore che indica se stampare pagine vuote di una visualizzazione
project.DefaultView.PageInfo.PageViewSettings.PrintBlankPages = false;

// imposta un valore che indica se stampare un numero specificato di prime colonne su tutte le pagine
project.DefaultView.PageInfo.PageViewSettings.PrintFirstColumnsCountOnAllPages = true;

project.Save(OutDir + "ProjectWithComments_out.pdf", SaveFileFormat.Pdf);
```

### Vedi anche

* class [PageViewSettings](../)
* namespace [Aspose.Tasks.Visualization](../../pageviewsettings/)
* assembly [Aspose.Tasks](../../../)


