---
title: "SaveOptions"
second_title: "Aspose.Tasks für Python via .NET API-Referenz"
description: 
type: docs
weight: 130
url: /de/python-net/aspose.tasks.saving/saveoptions/
---

## SaveOptions class

Dies ist eine abstrakte Basisklasse für Klassen, die dem Benutzer ermöglichen, zusätzliche Optionen beim Speichern eines Projekts<br/>            in ein bestimmtes Format anzugeben.

Der Typ SaveOptions stellt die folgenden Mitglieder bereit:
## Eigenschaften
| Name | Beschreibung |
| :- | :- |
| save_format | Ruft das Format ab oder legt es fest, in dem das Dokument gespeichert wird, wenn dieses Speicheroptionen-Objekt verwendet wird. |
| bar_styles | Liest oder setzt die Liste der Instanzen der Klasse [BarStyle](/tasks/python-net/aspose.tasks.visualization/barstyle/), die in der Projektansicht erscheinen. |
| draw_non_working_time | Liest oder setzt einen Wert, der angibt, ob Nichtarbeitszeit gezeichnet werden soll (Standardwert ist TRUE). |
| end_date | Liest oder setzt ein Datum, bis zu dem das Rendern abgeschlossen sein soll. |
| timescale_fit_behavior | Liest oder setzt ein Verhalten, das definiert, wie das rechte Ende der Zeitskala mit dem Seitenende ausgerichtet wird. |
| fit_content | Liest oder setzt einen Wert, der angibt, ob die Zeilenhöhe erhöht werden soll, um ihren Inhalt anzupassen. |
| gridlines | Liest oder setzt eine Liste von [Gridline](/tasks/python-net/aspose.tasks.visualization/gridline/), die in der Projektansicht erscheinen. |
| legend_drawing_options | Liest oder setzt einen Wert, der definiert, wie eine Legende gerendert wird. Standardwert ist LegendDrawingOptions.OnEveryPage. |
| legend_items | Liest oder setzt ein Array von PageLegendItem, das definiert, welche Balken in der Seitenlegende gerendert werden sollen.<br/>            Wenn null, werden die Standard‑Elemente gerendert. |
| mark_critical_tasks | Liest oder setzt einen Wert, der angibt, ob kritische Aufgaben in roter Farbe angezeigt werden sollen (Standardwert ist FALSE). |
| non_working_time_color | Liest oder setzt die Farbe der Nichtarbeitszeit. |
| page_count | Liest oder setzt die Anzahl der Seiten des Projekts. |
| page_size | Liest oder setzt die Größe der zu rendernden Seite (Standardwert ist PageSize.A4). |
| is_portrait | Liest oder setzt einen Wert, der angibt, ob die Seitenorientierung Hochformat ist; gibt false zurück, wenn die Seitenorientierung Querformat ist. |
| presentation_format | Liest oder setzt das [presentation_format](/tasks/python-net/aspose.tasks.saving/saveoptions/), in dem das Dokument gespeichert wird. |
| roll_up_gantt_bars | Liest oder setzt einen Wert, der angibt, ob Teilaufgaben in der Balkenanzeige der Zusammenfassungsaufgabe markiert werden sollen.<br/>            Für Teilaufgaben gibt das Rollup-Feld an, ob Informationen zu den Gantt-Balken der Teilaufgabe in den Balken der Zusammenfassungsaufgabe zusammengeführt werden.<br/>            Für Zusammenfassungsaufgaben gibt das Rollup-Feld an, ob der Balken der Zusammenfassungsaufgabe zusammengeführte Balken anzeigt.<br/>            Das Rollup-Feld für Zusammenfassungsaufgaben muss auf Ja gesetzt sein, damit Teilaufgaben zu ihnen zusammengeführt werden können. |
| start_date | Liest oder setzt das Datum, ab dem gerendert werden soll. |
| text_styles | Liest oder setzt die Liste der Textstile, die während der Darstellung einer Projektansicht angewendet werden. |
| timescale | Liest oder setzt den [timescale](/tasks/python-net/aspose.tasks.saving/saveoptions/) Wert, der verwendet wird, um zu steuern, wie die Zeitskala (falls vorhanden) gerendert wird, wenn das Projekt in ein grafisches Format gespeichert wird. |
| use_gradient_brush | Ruft einen Wert ab oder legt ihn fest, der angibt, ob ein Farbverlaufspinsel beim Rendern des Gantt-Diagramms verwendet werden soll. |
| view | Liest oder setzt eine Liste der Ansichtsspalten, die gerendert werden sollen ([GanttChartColumn](/tasks/python-net/aspose.tasks.visualization/ganttchartcolumn/)).<br/>            Wenn nicht gesetzt, werden nur Aufgaben-IDs, Aufgabennamen, Start und Ende gerendert.<br/>            Wenn sowohl View- als auch [view_settings](/tasks/python-net/aspose.tasks.saving/saveoptions/) Eigenschaften gesetzt sind, überschreiben die Spalten aus View die Spalten aus ViewSettings. |
| view_settings | Liest oder setzt eine Ansicht ([view](/tasks/python-net/aspose.tasks.saving/saveoptions/)) zum Rendern. Sie können diese Option verwenden, um explizit anzugeben, welche Ansicht in PDF-, HTML- oder Bildformate gespeichert werden soll.<br/>            Wenn diese Eigenschaft gesetzt ist, wird die [PresentationFormat](/tasks/python-net/aspose.tasks.visualization/presentationformat/) Eigenschaft beim Speichern des Projekts ignoriert.<br/>            Die Ansicht sollte von einem der folgenden Bildschirme stammen (([screen](/tasks/python-net/aspose.tasks/view/))): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage) |
| custom_page_size | Liest oder setzt die benutzerdefinierte Seitengröße in Punkten (1 Punkt = 1/72 Zoll). |
| render_to_single_page | Liest oder setzt einen Wert, der angibt, ob ein Projekt in einer einzelnen Seite gerendert werden soll<br/>            wenn das Projekt in einem grafischen Format gespeichert wird.<br/>            Die Seitengröße wird geändert, damit das gerenderte Projekt auf eine Seite passt. |

### Siehe auch

* namespace [aspose.tasks.saving](/tasks/python-net/aspose.tasks.saving/)
* assembly [Aspose.Tasks](/tasks/python-net/)

