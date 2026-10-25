---
title: "Aspose::Tasks::Saving::SaveOptions klasse"
linktitle: "SaveOptions"
articleTitle: "SaveOptions"
second_title: "Aspose.Tasks voor C++"
description: "Dit is een abstracte basisklasse voor klassen die de gebruiker in staat stelt extra opties op te geven bij het opslaan van een project in een bepaald formaat."
type: docs
weight: 10
url: /nl/cpp/aspose.tasks.saving/saveoptions/
---

## SaveOptions class

**Inherits:** Aspose::Tasks::Saving::SimpleSaveOptions

Dit is een abstracte basisklasse voor klassen die de gebruiker in staat stelt extra opties op te geven bij het opslaan van een project in een bepaald formaat.

Een instantie van een afgeleide klasse van de SaveOptions‑klasse wordt doorgegeven aan de stream‑Save‑ of string‑Save‑overloads zodat de gebruiker aangepaste opties kan definiëren bij het opslaan van een document.

## Methoden

| Naam | Beschrijving |
| --- | --- |
| [get_BarStyles](./get_barstyles/) | Haalt de lijst op van de instanties van de BarStyle‑klasse die in de projectweergave verschijnen. |
| [get_CustomPageSize](./get_custompagesize/) | Haalt de aangepaste paginagrootte op in points (1 point = 1/72 inch). |
| [get_DrawNonWorkingTime](./get_drawnonworkingtime/) | Haalt een waarde op die aangeeft of niet‑werkelijke tijd moet worden getekend (standaardwaarde is TRUE). |
| [get_EndDate](./get_enddate/) | Haalt een datum op waarop het renderen moet worden beëindigd. |
| [get_FitContent](./get_fitcontent/) | Haalt een waarde op die aangeeft of de rijhoogte moet worden vergroot om de inhoud te passen. |
| [get_FitTimescaleToEndOfPage](./get_fittimescaletoendofpage/) | Haalt op of een kalendersectie van een weergave tot het einde (rechterkant) van de laatste pagina moet worden gerenderd. Als de waarde false is, wordt de kalendersectie precies tot EndDate gerenderd, zelfs als er lege ruimte op een pagina is. |
| [get_Gridlines](./get_gridlines/) | Haalt een lijst op van Gridline die in de projectweergave verschijnen. |
| [get_IsPortrait](./get_isportrait/) | Haalt een waarde op die aangeeft of de paginarichting portrait is; retourneert false als de paginarichting landscape is. |
| [get_LegendDrawingOptions](./get_legenddrawingoptions/) | Haalt een waarde op die bepaalt hoe een legenda moet worden gerenderd. Standaardwaarde is LegendDrawingOptions.OnEveryPage. |
| [get_LegendItems](./get_legenditems/) | Haalt een array op van PageLegendItem die bepalen welke balken in de paginalegenda moeten worden gerenderd. Als null, worden de standaarditems gerenderd. |
| [get_MarkCriticalTasks](./get_markcriticaltasks/) | Haalt een waarde op die aangeeft of kritieke taken in rode kleur moeten worden weergegeven (standaardwaarde is FALSE). |
| [get_NonWorkingTimeColor](./get_nonworkingtimecolor/) | Haalt de kleur van niet‑werkelijke tijd op. |
| [get_PageCount](./get_pagecount/) | Haalt het aantal pagina's van het project op. |
| [get_PageSize](./get_pagesize/) | Haalt de grootte van de te renderen pagina op (standaardwaarde is PageSize.A4). |
| [get_PresentationFormat](./get_presentationformat/) | Haalt het PresentationFormat op waarin het document zal worden opgeslagen. |
| [get_RenderToSinglePage](./get_rendertosinglepage/) | Haalt een waarde op die aangeeft of een project op één pagina moet worden gerenderd wanneer het project wordt opgeslagen in een grafisch formaat. De paginagrootte wordt aangepast zodat het gerenderde project op één pagina past. |
| [get_RollUpGanttBars](./get_rollupganttbars/) | Haalt een waarde op die aangeeft of subtaken op de samenvattingsbalk gemarkeerd moeten worden. Voor subtaken geeft het Rollup‑veld aan of informatie over de Gantt‑balken van de subtaak wordt opgehoogd naar de samenvattingsbalk. Voor samenvattende taken geeft het Rollup‑veld aan of de samenvattingsbalk opgehoogde balken weergeeft. Het Rollup‑veld voor samenvattende taken moet op Ja staan om subtaken naar hen op te hogen. |
| [get_StartDate](./get_startdate/) | Haalt de datum op vanaf wanneer het renderen moet beginnen. |
| [get_TextStyles](./get_textstyles/) | Haalt de lijst op van tekststijlen die tijdens het renderen van een projectweergave worden toegepast. |
| [get_Timescale](./get_timescale/) | Haalt de Timescale‑waarde op die wordt gebruikt om te bepalen hoe de tijdschaal (indien aanwezig) wordt gerenderd wanneer het project wordt opgeslagen in een grafisch formaat. |
| [get_TimescaleFitBehavior](./get_timescalefitbehavior/) | Haalt een gedrag op dat bepaalt hoe het rechteruiteinde van de tijdschaal op het paginaword wordt uitgelijnd. |
| [get_UseGradientBrush](./get_usegradientbrush/) | Haalt een waarde op die aangeeft of een gradient‑kwast moet worden gebruikt bij het renderen van een Gantt‑diagram. |
| [get_View](./get_view/) | Haalt een lijst op van de weergavekolommen die moeten worden gerenderd ( GanttChartColumn ). Als dit niet is ingesteld, worden alleen taak‑ids, taaknamen, start en einde gerenderd. Als zowel View als ViewSettings properties zijn ingesteld, hebben kolommen van View voorrang op kolommen van ViewSettings. |
| [get_ViewSettings](./get_viewsettings/) | Haalt een weergave ( View ) op om te renderen. U kunt deze optie gebruiken om expliciet op te geven welke weergave moet worden opgeslagen in PDF-, HTML- of Image-formaten. Als deze eigenschap is ingesteld, wordt de Visualization::PresentationFormat‑eigenschap genegeerd wanneer het project wordt opgeslagen. View moet afkomstig zijn van een van de volgende schermen (( Aspose::Tasks::View::Screen )): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage). |
| [set_BarStyles](./set_barstyles/) | Stelt de lijst in van de instanties van de BarStyle‑klasse die in de projectweergave verschijnen. |
| [set_CustomPageSize](./set_custompagesize/) | Stelt de aangepaste paginagrootte in punten in (1 punt = 1/72 inch). |
| [set_DrawNonWorkingTime](./set_drawnonworkingtime/) | Stelt een waarde in die aangeeft of niet‑werkelijke tijd moet worden getekend (standaardwaarde is TRUE). |
| [set_EndDate](./set_enddate/) | Stelt een datum in waarop het renderen moet worden beëindigd. |
| [set_FitContent](./set_fitcontent/) | Stelt een waarde in die aangeeft of de rijhoogte moet worden vergroot om de inhoud te passen. |
| [set_FitTimescaleToEndOfPage](./set_fittimescaletoendofpage/) | Stelt in of een kalendersectie van een weergave tot het einde (rechterkant) van de laatste pagina moet worden gerenderd. Als de waarde false is, wordt de kalendersectie precies tot EndDate gerenderd, zelfs als er lege ruimte op een pagina is. |
| [set_Gridlines](./set_gridlines/) | Stelt een lijst in van Gridline die in de projectweergave verschijnen. |
| [set_IsPortrait](./set_isportrait/) | Stelt een waarde in die aangeeft of de paginarichting portret is; retourneert false als de paginarichting landschap is. |
| [set_LegendDrawingOptions](./set_legenddrawingoptions/) | Stelt een waarde in die bepaalt hoe een legenda moet worden gerenderd. Standaardwaarde is LegendDrawingOptions.OnEveryPage. |
| [set_LegendItems](./set_legenditems/) | Stelt een array in van PageLegendItem die bepalen welke balken in de paginalegenda moeten worden gerenderd. Als null, worden de standaarditems gerenderd. |
| [set_MarkCriticalTasks](./set_markcriticaltasks/) | Stelt een waarde in die aangeeft of kritieke taken in rode kleur moeten worden weergegeven (standaardwaarde is FALSE). |
| [set_NonWorkingTimeColor](./set_nonworkingtimecolor/) | Stelt de kleur voor niet‑werkelijke tijd in. |
| [set_PageSize](./set_pagesize/) | Stelt de grootte van de te renderen pagina in (standaardwaarde is PageSize.A4). |
| [set_PresentationFormat](./set_presentationformat/) | Stelt het PresentationFormat in waarin het document wordt opgeslagen. |
| [set_RenderToSinglePage](./set_rendertosinglepage/) | Stelt een waarde in die aangeeft of een project moet worden gerenderd op één pagina wanneer het project wordt opgeslagen in grafisch formaat. De paginagrootte wordt aangepast zodat het gerenderde project op één pagina past. |
| [set_RollUpGanttBars](./set_rollupganttbars/) | Stelt een waarde in die aangeeft of subtaken op de samenvattingsbalk gemarkeerd moeten worden. Voor subtaken geeft het Rollup‑veld aan of informatie over de subtaak‑Gantt‑balken wordt opgehoogd naar de samenvattingsbalk. Voor samenvattings‑taken geeft het Rollup‑veld aan of de samenvattingsbalk opgehoogde balken weergeeft. U moet het Rollup‑veld voor samenvattings‑taken op Ja hebben ingesteld zodat subtaken naar hen kunnen worden opgehoogd. |
| [set_StartDate](./set_startdate/) | Stelt de datum in waarop het renderen moet beginnen. |
| [set_TextStyles](./set_textstyles/) | Stelt de lijst in van tekststijlen die tijdens het renderen van een projectweergave worden toegepast. |
| [set_Timescale](./set_timescale/) | Stelt de Timescale‑waarde in die wordt gebruikt om te bepalen hoe de tijdschaal (indien aanwezig) wordt gerenderd wanneer het project wordt opgeslagen in grafisch formaat. |
| [set_TimescaleFitBehavior](./set_timescalefitbehavior/) | Stelt een gedrag in dat bepaalt hoe het rechteruiteinde van de tijdschaal wordt uitgelijnd met het einde van de pagina. |
| [set_UseGradientBrush](./set_usegradientbrush/) | Stelt een waarde in die aangeeft of een gradient‑brush moet worden gebruikt bij het renderen van een Gantt‑Chart. |
| [set_View](./set_view/) | Stelt een lijst in van de weergavekolommen die moeten worden gerenderd ( GanttChartColumn ). Als dit niet is ingesteld, worden alleen taak‑ids, taaknamen, start en einde gerenderd. Als zowel View als ViewSettings properties zijn ingesteld, hebben kolommen van View voorrang op kolommen van ViewSettings. |
| [set_ViewSettings](./set_viewsettings/) | Stelt een weergave ( View ) in om te renderen. U kunt deze optie gebruiken om expliciet op te geven welke weergave moet worden opgeslagen in PDF-, HTML- of Image-formaten. Als deze eigenschap is ingesteld, wordt de Visualization::PresentationFormat‑eigenschap genegeerd wanneer het project wordt opgeslagen. View moet afkomstig zijn van een van de volgende schermen (( Aspose::Tasks::View::Screen )): (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage). |

