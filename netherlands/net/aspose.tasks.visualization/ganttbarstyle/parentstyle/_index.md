---
title: "GanttBarStyle.ParentStyle"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "GanttBarStyle-eigenschap. Haalt op of stelt een bovenliggende of gemeenschappelijke stijl voor een aangepaste taak‑specifieke stijl in."
type: docs
weight: 160
url: /nl/net/aspose.tasks.visualization/ganttbarstyle/parentstyle/
---
## GanttBarStyle.ParentStyle property

Geeft of stelt een bovenliggende (of gemeenschappelijke) stijl in voor aangepaste taak‑specifieke stijl.

```csharp
public GanttBarStyle ParentStyle { get; set; }
```

## Opmerkingen

Een taak kan meerdere aangepaste stijlen hebben met verschillende bovenliggende stijlen. Bijvoorbeeld, beschouw een taak met een aangepaste stijl met de bovenliggende stijl "Critical" en een andere stijl met de bovenliggende stijl "Normal". Simpel gezegd, als de taak kritisch is, wordt de eerste stijl toegepast. Als de taak niet‑kritisch wordt, wordt de tweede stijl toegepast (deze logica is geërfd van Microsoft Project Professional).

## Voorbeelden

Toont hoe aangepaste balkstijlen van een weergave gelezen kunnen worden.

```csharp
var project = new Project(DataDir + "CustomBarStyle.mpp");

var view = (GanttChartView)project.DefaultView;
Console.WriteLine("Custom bar styles count: {0}", view.CustomBarStyles.Count);

var style1 = view.CustomBarStyles[0];
Console.WriteLine("Style1.ParentStyle Name: {0}", style1.ParentStyle.Name);
Console.WriteLine("Style1.LeftField: {0}", style1.LeftField);
Console.WriteLine("Style1.RightField: {0}", style1.RightField);
Console.WriteLine("Style1.TopField: {0}", style1.TopField);
Console.WriteLine("Style1.BottomField: {0}", style1.BottomField);
Console.WriteLine("Style1.InsideField: {0}", style1.InsideField);
Console.WriteLine("Style1.From: {0}", style1.From);
Console.WriteLine("Style1.To: {0}", style1.To);
Console.WriteLine("Style1.Row: {0}", style1.Row);

var style2 = view.CustomBarStyles[1];
Console.WriteLine("Style2.LeftField: {0}", style2.LeftField);
Console.WriteLine("Style2.RightField: {0}", style2.RightField);
Console.WriteLine("Style2.TopField: {0}", style2.TopField);
Console.WriteLine("Style2.BottomField: {0}", style2.BottomField);
Console.WriteLine("Style2.InsideField: {0}", style2.InsideField);
Console.WriteLine("Style2.From: {0}", style2.From);
Console.WriteLine("Style2.To: {0}", style2.To);
Console.WriteLine("Style2.Row: {0}", style1.Row);

var style3 = view.CustomBarStyles[2];
Console.WriteLine("Style3.LeftField: {0}", style3.LeftField);
Console.WriteLine("Style3.RightField: {0}", style3.RightField);
Console.WriteLine("Style3.TopField: {0}", style3.TopField);
Console.WriteLine("Style3.BottomField: {0}", style3.BottomField);
Console.WriteLine("Style3.InsideField: {0}", style3.InsideField);

Console.WriteLine("Style3.StartShape: {0}", style3.StartShape);
Console.WriteLine("Style3.StartShapeType: {0}", style3.StartShapeType);
Console.WriteLine("Style3.StartShapeColor: {0}", style3.StartShapeColor);

Console.WriteLine("Style3.EndShape: {0}", style3.EndShape);
Console.WriteLine("Style3.EndShapeType: {0}", style3.EndShapeType);
Console.WriteLine("Style3.EndShapeColor: {0}", style3.EndShapeColor);

Console.WriteLine("Style3.MiddleShape: {0}", style3.MiddleShape);
Console.WriteLine("Style3.MiddleFillPattern: {0}", style3.MiddleFillPattern);
Console.WriteLine("Style3.MiddleShapeColor: {0}", style3.MiddleShapeColor);
Console.WriteLine("Style3.From: {0}", style3.From);
Console.WriteLine("Style3.To: {0}", style3.To);
Console.WriteLine("Style3.Row: {0}", style1.Row);
```

### Zie ook

* class [GanttBarStyle](../)
* namespace [Aspose.Tasks.Visualization](../../ganttbarstyle/)
* assembly [Aspose.Tasks](../../../)


