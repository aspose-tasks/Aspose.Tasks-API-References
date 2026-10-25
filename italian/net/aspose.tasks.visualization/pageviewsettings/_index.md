---
title: "Classe PageViewSettings"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Aspose.Tasks.Visualization.PageViewSettings classe. Rappresenta le impostazioni di stampa per una visualizzazione del progetto"
type: docs
weight: 3260
url: /it/net/aspose.tasks.visualization/pageviewsettings/
---
## PageViewSettings class

Rappresenta le impostazioni di stampa per una visualizzazione del progetto.

```csharp
public class PageViewSettings
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [PageViewSettings](pageviewsettings/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [FirstColumnsCount](../../aspose.tasks.visualization/pageviewsettings/firstcolumnscount/) { get; set; } | Ottiene o imposta il numero delle prime colonne da stampare su tutte le pagine. |
| [FitTimescaleToEndOfPage](../../aspose.tasks.visualization/pageviewsettings/fittimescaletoendofpage/) { get; set; } | Ottiene o imposta un valore che indica se adattare la scala temporale alla fine di una pagina durante la stampa. |
| [PrintAllSheetColumns](../../aspose.tasks.visualization/pageviewsettings/printallsheetcolumns/) { get; set; } | Ottiene o imposta un valore che indica se stampare tutte le colonne del foglio di una visualizzazione. |
| [PrintBlankPages](../../aspose.tasks.visualization/pageviewsettings/printblankpages/) { get; set; } | Ottiene o imposta un valore che indica se stampare pagine vuote di una visualizzazione. |
| [PrintFirstColumnsCountOnAllPages](../../aspose.tasks.visualization/pageviewsettings/printfirstcolumnscountonallpages/) { get; set; } | Ottiene o imposta un valore che indica se stampare un numero specificato di prime colonne su tutte le pagine. |
| [PrintNotes](../../aspose.tasks.visualization/pageviewsettings/printnotes/) { get; set; } | Ottiene o imposta un valore che indica se stampare le note. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


