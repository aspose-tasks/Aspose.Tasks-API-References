---
title: "TableTextStyle.Field"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "TableTextStyle eigenschap. Haalt of stelt een veld in waarop de stijl moet worden toegepast. Field"
type: docs
weight: 20
url: /nl/net/aspose.tasks.visualization/tabletextstyle/field/
---
## TableTextStyle.Field property

Haalt of stelt een veld in waarop de stijl moet worden toegepast. `Field`.

```csharp
public Field Field { get; set; }
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

* enum [Field](../../../aspose.tasks/field/)
* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)


