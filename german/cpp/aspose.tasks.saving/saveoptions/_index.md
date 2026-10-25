---
title: "Aspose::Tasks::Saving::SaveOptions Klasse"
linktitle: "SaveOptions"
articleTitle: "SaveOptions"
second_title: "Aspose.Tasks für C++"
description: "Dies ist eine abstrakte Basisklasse für Klassen, die es dem Benutzer ermöglichen, zusätzliche Optionen beim Speichern eines Projekts in ein bestimmtes Format anzugeben."
type: docs
weight: 10
url: /de/cpp/aspose.tasks.saving/saveoptions/
---

## SaveOptions class

**Inherits:** Aspose::Tasks::Saving::SimpleSaveOptions

Dies ist eine abstrakte Basisklasse für Klassen, die es dem Benutzer ermöglichen, zusätzliche Optionen beim Speichern eines Projekts in ein bestimmtes Format anzugeben.

Eine Instanz einer beliebigen von der SaveOptions‑Klasse abgeleiteten Klasse wird an die Stream‑Save‑ oder String‑Save‑Überladungen übergeben, damit der Benutzer benutzerdefinierte Optionen beim Speichern eines Dokuments festlegen kann.

## Methoden

| Name | Beschreibung |
| --- | --- |
| [get_BarStyles](./get_barstyles/) | Gibt die Liste der Instanzen der BarStyle‑Klasse zurück, die in der Projektansicht erscheinen. |
| [get_CustomPageSize](./get_custompagesize/) | Gibt die benutzerdefinierte Seitengröße in Punkten zurück (1 Punkt = 1/72 Zoll). |
| [get_DrawNonWorkingTime](./get_drawnonworkingtime/) | Gibt einen Wert zurück, der angibt, ob Nichtarbeitszeit gezeichnet werden soll (Standardwert ist TRUE). |
| [get_EndDate](./get_enddate/) | Gibt ein Datum zurück, bis zu dem gerendert werden soll. |
| [get_FitContent](./get_fitcontent/) | Gibt einen Wert zurück, der angibt, ob die Zeilenhöhe erhöht werden soll, um ihren Inhalt anzupassen. |
| [get_FitTimescaleToEndOfPage](./get_fittimescaletoendofpage/) | Gibt an, ob ein Kalenderabschnitt einer Ansicht bis zum Ende (rechte Seite) der letzten Seite gerendert werden soll. Wenn der Wert false ist, wird der Kalenderabschnitt exakt bis zum Enddatum gerendert, selbst wenn auf einer Seite ein leerer Raum verbleibt. |
| [get_Gridlines](./get_gridlines/) | Gibt eine Liste von Gridline zurück, die in der Projektansicht erscheinen. |
| [get_IsPortrait](./get_isportrait/) | Gibt einen Wert zurück, der angibt, ob die Seitenausrichtung Hochformat ist; gibt false zurück, wenn die Seitenausrichtung Querformat ist. |
| [get_LegendDrawingOptions](./get_legenddrawingoptions/) | Gibt einen Wert zurück, der definiert, wie eine Legende gerendert wird. Standardwert ist LegendDrawingOptions.OnEveryPage. |
| [get_LegendItems](./get_legenditems/) | Gibt ein Array von PageLegendItem zurück, das definiert, welche Balken in der Seitenlegende gerendert werden sollen. Wenn null, werden die Standard‑Elemente gerendert. |
| [get_MarkCriticalTasks](./get_markcriticaltasks/) | Gibt einen Wert zurück, der angibt, ob kritische Aufgaben in roter Farbe angezeigt werden sollen (Standardwert ist FALSE). |
| [get_NonWorkingTimeColor](./get_nonworkingtimecolor/) | Gibt die Farbe der Nichtarbeitszeit zurück. |
| [get_PageCount](./get_pagecount/) | Gibt die Anzahl der Seiten des Projekts zurück. |
| [get_PageSize](./get_pagesize/) | Gibt die Größe der zu rendernden Seite zurück (Standardwert ist PageSize.A4). |
| [get_PresentationFormat](./get_presentationformat/) | Gibt das PresentationFormat zurück, in dem das Dokument gespeichert wird. |
| [get_RenderToSinglePage](./get_rendertosinglepage/) | Gibt einen Wert zurück, der angibt, ob ein Projekt in einer einzelnen Seite gerendert werden soll, wenn das Projekt im grafischen Format gespeichert wird. Die Seitengröße wird geändert, damit das gerenderte Projekt auf eine Seite passt. |
| [get_RollUpGanttBars](./get_rollupganttbars/) | Gibt einen Wert zurück, der angibt, ob Teilaufgaben auf der Balken‑Zusammenfassungsleiste markiert werden sollen. Für Teilaufgaben gibt das Rollup‑Feld an, ob Informationen zu den Gantt‑Balken der Teilaufgabe in die Zusammenfassungsleiste übernommen werden. Für Zusammenfassungsaufgaben gibt das Rollup‑Feld an, ob die Zusammenfassungsleiste gerollte Balken anzeigt. Das Rollup‑Feld für Zusammenfassungsaufgaben muss auf Ja gesetzt sein, damit Teilaufgaben zu ihnen hochgerollt werden können. |
| [get_StartDate](./get_startdate/) | Gibt das Datum zurück, ab dem gerendert werden soll. |
| [get_TextStyles](./get_textstyles/) | Gibt die Liste der Textstile zurück, die während des Renderns einer Projektansicht angewendet werden. |
| [get_Timescale](./get_timescale/) | Gibt den Timescale‑Wert zurück, der verwendet wird, um zu steuern, wie die Zeitskala (falls vorhanden) gerendert wird, wenn das Projekt im grafischen Format gespeichert wird. |
| [get_TimescaleFitBehavior](./get_timescalefitbehavior/) | Gibt ein Verhalten zurück, das definiert, wie das rechte Ende der Zeitskala mit dem Seitenende ausgerichtet wird. |
| [get_UseGradientBrush](./get_usegradientbrush/) | Gibt einen Wert zurück, der angibt, ob ein Farbverlaufspinsel beim Rendern des Gantt‑Diagramms verwendet werden soll. |
| [get_View](./get_view/) | Gibt eine Liste der Ansichtsspalten zurück, die gerendert werden sollen ( GanttChartColumn ). Wenn nicht festgelegt, werden nur Aufgaben‑IDs, Aufgabennamen, Start‑ und Endzeit gerendert. Wenn sowohl die Eigenschaften View als auch ViewSettings gesetzt sind, überschreiben die Spalten aus View die Spalten aus ViewSettings. |
| [get_ViewSettings](./get_viewsettings/) | Gibt eine Ansicht ( View ) zurück, die gerendert werden soll. Sie können diese Option verwenden, um explizit anzugeben, welche Ansicht in PDF-, HTML- oder Bildformate gespeichert werden soll. Wenn diese Eigenschaft gesetzt ist, wird die Eigenschaft Visualization::PresentationFormat beim Speichern des Projekts ignoriert. Die Ansicht muss von einem der folgenden Bildschirme (( Aspose::Tasks::View::Screen )) stammen: (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage). |
| [set_BarStyles](./set_barstyles/) | Legt die Liste der Instanzen der Klasse BarStyle fest, die in der Projektansicht erscheinen. |
| [set_CustomPageSize](./set_custompagesize/) | Legt die benutzerdefinierte Seitengröße in Punkten fest (1 Punkt = 1/72 Zoll). |
| [set_DrawNonWorkingTime](./set_drawnonworkingtime/) | Legt einen Wert fest, der angibt, ob Nichtarbeitszeit gezeichnet werden soll (Standardwert ist TRUE). |
| [set_EndDate](./set_enddate/) | Legt ein Datum fest, bis zu dem das Rendering beendet werden soll. |
| [set_FitContent](./set_fitcontent/) | Legt einen Wert fest, der angibt, ob die Zeilenhöhe erhöht werden soll, um ihren Inhalt anzupassen. |
| [set_FitTimescaleToEndOfPage](./set_fittimescaletoendofpage/) | Legt fest, ob ein Kalenderabschnitt einer Ansicht bis zum Ende (rechte Seite) der letzten Seite gerendert werden soll. Wenn der Wert false ist, wird der Kalenderabschnitt exakt bis zum Enddatum gerendert, selbst wenn auf einer Seite ein leerer Raum verbleibt. |
| [set_Gridlines](./set_gridlines/) | Legt eine Liste von Gridline fest, die in der Projektansicht erscheinen. |
| [set_IsPortrait](./set_isportrait/) | Legt einen Wert fest, der angibt, ob die Seitenausrichtung Hochformat ist; gibt false zurück, wenn die Seitenausrichtung Querformat ist. |
| [set_LegendDrawingOptions](./set_legenddrawingoptions/) | Legt einen Wert fest, der definiert, wie eine Legende gerendert wird. Standardwert ist LegendDrawingOptions.OnEveryPage. |
| [set_LegendItems](./set_legenditems/) | Legt ein Array von PageLegendItem fest, das definiert, welche Balken in der Seitenlegende gerendert werden sollen. Wenn null, werden die Standard‑Elemente gerendert. |
| [set_MarkCriticalTasks](./set_markcriticaltasks/) | Legt einen Wert fest, der angibt, ob kritische Aufgaben in roter Farbe angezeigt werden sollen (Standardwert ist FALSE). |
| [set_NonWorkingTimeColor](./set_nonworkingtimecolor/) | Legt die Farbe für Nichtarbeitszeit fest. |
| [set_PageSize](./set_pagesize/) | Legt die Größe der zu rendernden Seite fest (Standardwert ist PageSize.A4). |
| [set_PresentationFormat](./set_presentationformat/) | Legt das PresentationFormat fest, in dem das Dokument gespeichert wird. |
| [set_RenderToSinglePage](./set_rendertosinglepage/) | Legt einen Wert fest, der angibt, ob ein Projekt in einer einzelnen Seite gerendert werden soll, wenn das Projekt im grafischen Format gespeichert wird. Die Seitengröße wird angepasst, sodass das gerenderte Projekt auf eine Seite passt. |
| [set_RollUpGanttBars](./set_rollupganttbars/) | Legt einen Wert fest, der angibt, ob Teilaufgaben in der Balkenanzeige der Zusammenfassungsaufgabe markiert werden sollen. Für Teilaufgaben gibt das Feld Rollup an, ob Informationen zu den Gantt‑Balken der Teilaufgabe in den Balken der Zusammenfassungsaufgabe zusammengefasst werden. Für Zusammenfassungsaufgaben gibt das Feld Rollup an, ob der Balken der Zusammenfassungsaufgabe zusammengefasste Balken anzeigt. Das Feld Rollup für Zusammenfassungsaufgaben muss auf Ja gesetzt sein, damit Teilaufgaben zu ihnen zusammengefasst werden können. |
| [set_StartDate](./set_startdate/) | Legt das Datum fest, ab dem das Rendering beginnen soll. |
| [set_TextStyles](./set_textstyles/) | Legt die Liste der Textstile fest, die beim Rendern einer Projektansicht angewendet werden. |
| [set_Timescale](./set_timescale/) | Legt den Timescale‑Wert fest, der verwendet wird, um zu steuern, wie die Zeitskala (falls vorhanden) beim Speichern des Projekts im grafischen Format gerendert wird. |
| [set_TimescaleFitBehavior](./set_timescalefitbehavior/) | Legt ein Verhalten fest, das definiert, wie das rechte Ende der Zeitskala mit dem Seitenende ausgerichtet wird. |
| [set_UseGradientBrush](./set_usegradientbrush/) | Legt einen Wert fest, der angibt, ob ein Farbverlaufspinsel beim Rendern des Gantt‑Diagramms verwendet werden soll. |
| [set_View](./set_view/) | Legt eine Liste der anzuzeigenden Ansichtsspalten fest ( GanttChartColumn ). Wenn nicht festgelegt, werden nur Aufgaben‑IDs, Aufgabennamen, Start und Ende gerendert. Wenn sowohl die Eigenschaften View als auch ViewSettings festgelegt sind, überschreiben die Spalten aus View die Spalten aus ViewSettings. |
| [set_ViewSettings](./set_viewsettings/) | Legt eine Ansicht ( View ) fest, die gerendert werden soll. Sie können diese Option verwenden, um explizit anzugeben, welche Ansicht in PDF-, HTML- oder Bildformate gespeichert werden soll. Wenn diese Eigenschaft festgelegt ist, wird die Eigenschaft Visualization::PresentationFormat beim Speichern des Projekts ignoriert. Die Ansicht muss von einem der folgenden Bildschirme (( Aspose::Tasks::View::Screen )) stammen: (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage). |

