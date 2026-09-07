---
title: "Classe TableField"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.TableField. Rappresenta un campo di una tabella in un progetto"
type: docs
weight: 2340
url: /it/net/aspose.tasks/tablefield/
---
## TableField class

Rappresenta un campo di una tabella in un progetto.

```csharp
public class TableField
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [TableField](tablefield/)() | Inizializza una nuova istanza della classe `TableField`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [AlignData](../../aspose.tasks/tablefield/aligndata/) { get; set; } | Ottiene o imposta l'allineamento dei dati in un campo della tabella. |
| [AlignTitle](../../aspose.tasks/tablefield/aligntitle/) { get; set; } | Ottiene o imposta l'allineamento del titolo in un campo della tabella. |
| [Field](../../aspose.tasks/tablefield/field/) { get; set; } | Ottiene o imposta il tipo di un campo della tabella. |
| [Title](../../aspose.tasks/tablefield/title/) { get; set; } | Ottiene o imposta il titolo del campo in una tabella. |
| [Width](../../aspose.tasks/tablefield/width/) { get; set; } | Ottiene o imposta la larghezza in punti della colonna del campo in una tabella. |
| [WrapHeader](../../aspose.tasks/tablefield/wrapheader/) { get; set; } | Ottiene o imposta un valore che indica se l'intestazione della colonna della tabella può andare a capo su più righe, o se deve essere troncata quando supera la larghezza della colonna. |
| [WrapText](../../aspose.tasks/tablefield/wraptext/) { get; set; } | Ottiene o imposta un valore che indica se il testo della colonna può andare a capo su più righe, o se deve essere troncato quando supera la larghezza della colonna. Supportato dalla versione MSP 2010 e successive. |

## Esempi

Mostra come lavorare con la vista di Project e aggiungere una colonna alla vista predefinita (che viene mostrata quando un file MPP è aperto in MS Project).

```csharp
// crea un progetto vuoto senza viste
var project = new Project();
project.Set(Prj.Name, "Test View Project");

// Modifica la vista predefinita (è una vista diagramma di Gantt).
// Oppure puoi selezionare la vista per nome o tramite la schermata Vista usando la collezione project.View.
var view = (GanttChartView) project.DefaultView;

TableField newColumn = new TableField()
{
    AlignData = HorizontalStringAlignment.Center,
    Title = "My new column",
    Width = 30,
    Field = Field.TaskActualDuration
};

view.Table.TableFields.Add(newColumn);

// Il flag WriteViewData dovrebbe essere usato per persistere le modifiche alle proprietà della vista.
project.Save(OutDir + "ModifyView_output.mpp", new Saving.MPPSaveOptions
{
    WriteViewData = true
});
```

Mostra come leggere le tabelle del progetto.

```csharp
var project = new Project(DataDir + "ReadTableData.mpp");

// ottieni la tabella
var table = project.Tables.ToList()[0];
Console.WriteLine("Print table fields of {0}", table.Name);
Console.WriteLine("Table Fields Count" + table.TableFields.Count);

// visualizza le informazioni di tutti i campi della tabella
foreach (var field in table.TableFields)
{
    Console.WriteLine("  Field: " + field.Field);
    Console.WriteLine("  Width: " + field.Width);
    Console.WriteLine("  Title: " + field.Title);
    Console.WriteLine("  Title Alignment: " + field.AlignTitle);
    Console.WriteLine("  Data Alignment: " + field.AlignData);
    Console.WriteLine("  Wrap Header: " + field.WrapHeader);
    Console.WriteLine("  Wrap Text: " + field.WrapText);
    Console.WriteLine();
}
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


