---
title: XamlOptions
second_title: Aspose.Tasks für .NET-API-Referenz
description: /// Ermöglicht die Angabe zusätzlicher Optionen beim Rendern von Projektseiten in XAML.
type: docs
weight: 1960
url: /de/net/aspose.tasks.saving/xamloptions/
---
## XamlOptions class

/// Ermöglicht die Angabe zusätzlicher Optionen beim Rendern von Projektseiten in XAML.

```csharp
public class XamlOptions : SaveOptions
```

## Konstrukteure

| Name | Beschreibung |
| --- | --- |
| [XamlOptions](xamloptions)() | Initialisiert eine neue Instanz von[`XamlOptions`](../xamloptions) Klasse, die zum Speichern von Projekten im XAML-Format verwendet werden kann. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [BarStyles](../../aspose.tasks.saving/saveoptions/barstyles) { get; set; } | Ruft die Liste der Instanzen von ab oder legt sie fest[`BarStyle`](../../aspose.tasks.visualization/barstyle) Klasse, die in der Projektansicht angezeigt werden. |
| [CustomPageSize](../../aspose.tasks.saving/saveoptions/custompagesize) { get; set; } | Ruft die benutzerdefinierte Seitengröße in Punkt ab oder legt sie fest (1 Punkt = 1/72 Zoll). |
| [DrawNonWorkingTime](../../aspose.tasks.saving/saveoptions/drawnonworkingtime) { get; set; } | Ruft oder setzt einen Wert, der angibt, ob arbeitsfreie Zeit gezogen werden soll (Standardwert ist TRUE). |
| [EndDate](../../aspose.tasks.saving/saveoptions/enddate) { get; set; } | Ruft ein Datum ab, an dem das Rendern beendet werden soll, oder legt es fest. |
| [FitContent](../../aspose.tasks.saving/saveoptions/fitcontent) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob die Zeilenhöhe erhöht werden soll, um sie an den Inhalt anzupassen. |
| [Gridlines](../../aspose.tasks.saving/saveoptions/gridlines) { get; set; } | Holt oder setzt eine Liste von[`Gridline`](../../aspose.tasks.visualization/gridline) die in der Projektansicht erscheinen. |
| [LegendOnEachPage](../../aspose.tasks.saving/saveoptions/legendoneachpage) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob die Legende auf jeder Seite angezeigt werden soll (Standardwert ist TRUE). |
| [MarkCriticalTasks](../../aspose.tasks.saving/saveoptions/markcriticaltasks) { get; set; } | Ruft oder setzt einen Wert, der angibt, ob kritische Aufgaben in roter Farbe angezeigt werden sollen (Standardwert ist FALSE). |
| [NonWorkingTimeColor](../../aspose.tasks.saving/saveoptions/nonworkingtimecolor) { get; set; } | Ruft die Farbe der arbeitsfreien Zeit ab oder legt sie fest. |
| [PageCount](../../aspose.tasks.saving/saveoptions/pagecount) { get; } | Ruft die Anzahl der Projektseiten ab oder legt sie fest. |
| [PageSize](../../aspose.tasks.saving/saveoptions/pagesize) { get; set; } | Ruft die Größe der darzustellenden Seite ab oder legt sie fest (Standardwert ist PageSize.A4). |
| [PresentationFormat](../../aspose.tasks.saving/saveoptions/presentationformat) { get; set; } | Ruft ab oder setzt die[`PresentationFormat`](../saveoptions/presentationformat) in dem das Dokument gespeichert wird. |
| [RenderToSinglePage](../../aspose.tasks.saving/saveoptions/rendertosinglepage) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob ein Projekt auf einer einzelnen Seite gerendert werden soll, wenn das Projekt im grafischen Format gespeichert wird. Die Seitengröße wird geändert, damit das gerenderte Projekt auf eine Seite passt. |
| [RollUpGanttBars](../../aspose.tasks.saving/saveoptions/rollupganttbars) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob Teilvorgänge auf der Sammelvorgangsleiste markiert werden sollen. Für Teilvorgänge gibt das Rollup-Feld an, ob Informationen zu den Teilvorgangs-Gantt-Balken in die Sammelvorgangsleiste hochgerollt werden. Für Sammelvorgänge das Rollup Feld gibt an, ob die Sammelvorgangsleiste Rollup-Balken anzeigt. Sie müssen das Rollup-Feld für Sammelvorgänge auf Ja gesetzt haben, damit Untervorgänge zu ihnen zusammengefasst werden können. |
| [SaveFormat](../../aspose.tasks.saving/saveoptions/saveformat) { get; } | Ruft das Format ab oder legt es fest, in dem das Dokument gespeichert wird, wenn dieses Speicheroptionsobjekt verwendet wird. |
| [StartDate](../../aspose.tasks.saving/saveoptions/startdate) { get; set; } | Ruft das Datum ab, an dem das Rendern beginnen soll, oder legt es fest. |
| [TasksComparer](../../aspose.tasks.saving/saveoptions/taskscomparer) { get; set; } | Ruft den Vergleicher ab oder legt ihn fest, um Aufgaben im Gantt-Diagramm und im Aufgabenblattdiagramm zu sortieren. |
| [TasksFilter](../../aspose.tasks.saving/saveoptions/tasksfilter) { get; set; } | Ruft die Bedingung ab oder legt sie fest, die verwendet wird, um Aufgaben zu filtern, die in Gantt-, Aufgabenblatt- und Aufgabenverwendungsdiagrammen gerendert werden. |
| [TextStyles](../../aspose.tasks.saving/saveoptions/textstyles) { get; set; } | Ruft die Liste der Instanzen von ab oder legt sie fest[`TextStyle`](../../aspose.tasks.visualization/textstyle) Klasse, die in der Projektansicht angezeigt werden. |
| [Timescale](../../aspose.tasks.saving/saveoptions/timescale) { get; set; } | Ruft ab oder setzt die[`Timescale`](../saveoptions/timescale) Wert, der verwendet wird, um zu steuern, wie die Zeitskala (falls vorhanden) gerendert wird, wenn das Projekt im grafischen Format gespeichert wird. |
| virtual [UseGradientBrush](../../aspose.tasks.saving/saveoptions/usegradientbrush) { get; set; } | Ruft einen Wert ab oder legt einen Wert fest, der angibt, ob beim Rendern von Gantt-Diagrammen ein Verlaufspinsel verwendet werden soll. |
| [View](../../aspose.tasks.saving/saveoptions/view) { get; set; } | Ruft eine Liste der zu rendernden Ansichtsspalten ab oder legt sie fest ([`GanttChartColumn`](../../aspose.tasks.visualization/ganttchartcolumn) ). Wenn nicht festgelegt, werden nur Aufgaben-IDs, Aufgabennamen, Start und Ende gerendert. Wenn sowohl Ansicht als auch[`ViewSettings`](../saveoptions/viewsettings) Eigenschaften festgelegt sind, Spalten von View überschreiben Spalten von ViewSettings. |
| [ViewSettings](../../aspose.tasks.saving/saveoptions/viewsettings) { get; set; } | Ruft eine Ansicht ab oder legt sie fest ([`View`](../saveoptions/view) zu rendern. Mit diesen Optionen können Sie explizit angeben, welche Ansicht im PDF-, HTML- oder Bildformat gespeichert werden soll. Wenn diese Eigenschaft gesetzt ist,[`PresentationFormat`](../../aspose.tasks.visualization/presentationformat) Die Eigenschaft wird beim Speichern des Projekts ignoriert. Die Ansicht sollte von einem der folgenden Bildschirme erfolgen (([`Screen`](../../aspose.tasks/view/screen) )): (Gantt, Aufgabenblatt, Aufgabennutzung, Ressourcenblatt, Ressourcennutzung) |

### Siehe auch

* class [SaveOptions](../saveoptions)
* namensraum [Aspose.Tasks.Saving](../../aspose.tasks.saving)
* Montage [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
