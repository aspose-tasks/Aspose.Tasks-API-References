---
title: "Klasse TableField"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.TableField klasse. Vertegenwoordigt een veld van een tabel in een project."
type: docs
weight: 2340
url: /nl/net/aspose.tasks/tablefield/
---
## TableField class

Stelt een veld van een tabel in een project voor.

```csharp
public class TableField
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [TableField](tablefield/)() | Initialiseert een nieuw exemplaar van de `TableField` klasse. |

## Eigenschappen

| Naam | Beschrijving |
| --- | --- |
| [AlignData](../../aspose.tasks/tablefield/aligndata/) { get; set; } | Haalt op of stelt de uitlijning van gegevens in een tabelveld in. |
| [AlignTitle](../../aspose.tasks/tablefield/aligntitle/) { get; set; } | Haalt op of stelt de uitlijning van de titel in een tabelveld in. |
| [Field](../../aspose.tasks/tablefield/field/) { get; set; } | Haalt op of stelt het type van een tabelveld in. |
| [Title](../../aspose.tasks/tablefield/title/) { get; set; } | Haalt op of stelt de titel van het veld in een tabel in. |
| [Width](../../aspose.tasks/tablefield/width/) { get; set; } | Haalt op of stelt de breedte in punten van de veldkolom in een tabel in. |
| [WrapHeader](../../aspose.tasks/tablefield/wrapheader/) { get; set; } | Haalt op of stelt een waarde in die aangeeft of de kolomkop van de tabel kan worden afgebroken over meerdere regels, of dat deze moet worden afgekapt wanneer deze de kolombreedte overschrijdt. |
| [WrapText](../../aspose.tasks/tablefield/wraptext/) { get; set; } | Haalt een waarde op of stelt deze in die aangeeft of de kolomtekst kan worden afgebroken over meerdere regels, of dat deze moet worden afgekapt wanneer deze de kolombreedte overschrijdt. Ondersteund door versie MSP 2010 en later. |

## Voorbeelden

Toont hoe te werken met de weergave van Project en een kolom toe te voegen aan de standaardweergave (die wordt weergegeven wanneer een MPP‑bestand wordt geopend in MS Project).

```csharp
// maak een leeg project zonder weergaven
var project = new Project();
project.Set(Prj.Name, "Test View Project");

// Wijzig de standaardweergave (het is een Gantt‑diagramweergave).
// Of je kunt de weergave selecteren op naam of via het View‑scherm met behulp van de project.View‑collectie.
var view = (GanttChartView) project.DefaultView;

TableField newColumn = new TableField()
{
    AlignData = HorizontalStringAlignment.Center,
    Title = "My new column",
    Width = 30,
    Field = Field.TaskActualDuration
};

view.Table.TableFields.Add(newColumn);

// De WriteViewData‑vlag moet worden gebruikt om wijzigingen in de eigenschappen van de weergave te behouden.
project.Save(OutDir + "ModifyView_output.mpp", new Saving.MPPSaveOptions
{
    WriteViewData = true
});
```

Toont hoe projecttabellen te lezen.

```csharp
var project = new Project(DataDir + "ReadTableData.mpp");

// haal de tabel op
var table = project.Tables.ToList()[0];
Console.WriteLine("Print table fields of {0}", table.Name);
Console.WriteLine("Table Fields Count" + table.TableFields.Count);

// geef alle informatie van tabelvelden weer
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

### Zie ook

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


