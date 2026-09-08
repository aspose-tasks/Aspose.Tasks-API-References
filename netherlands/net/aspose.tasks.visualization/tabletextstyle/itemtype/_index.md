---
title: "TableTextStyle.ItemType"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "TableTextStyle eigenschap. Retourneert een waarde van de TextItemType‑enum."
type: docs
weight: 30
url: /nl/net/aspose.tasks.visualization/tabletextstyle/itemtype/
---
## TableTextStyle.ItemType property

Retourneert een waarde van de [`TextItemType`](../../textitemtype/) enum.

```csharp
public override TextItemType ItemType { get; }
```

## Voorbeelden

Toont hoe tabeltekststijlen kunnen worden aangepast die worden gebruikt om verschillende tekstitems in een project te stijlen.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.NewTasksAreManual, false);

var view = (GanttChartView)project.Views.ToList()[0];

// stel eerste taaknaam tekststijl in
var style1 = new TableTextStyle(1);
// stel een veld in waarop de stijl moet worden toegepast.
style1.Field = Field.TaskName;
// stel <see cref="P:Aspose.Tasks.Visualization.TextStyle.Font" /> van de tekststijl in.
style1.Font = new FontDescriptor("Impact", 12F, FontStyles.Bold | FontStyles.Italic);
// stel grootte in punten van het lettertype van de tekststijl in.

// stel tweede taakduur tekststijl in
var style2 = new TableTextStyle(2);
style2.Field = Field.TaskDurationText;
style2.Font = new FontDescriptor("Impact", 16F, FontStyles.Underline);

view.TableTextStyles.Add(style1);
view.TableTextStyles.Add(style2);

SimpleSaveOptions options = new MPPSaveOptions
{
    // stel een vlag in die aangeeft dat weergavegegevens moeten worden geschreven
    WriteViewData = true
};
project.Save(OutDir + "WorkWithTableTextStyle_out.mpp", options);
```

### Zie ook

* enum [TextItemType](../../textitemtype/)
* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)


