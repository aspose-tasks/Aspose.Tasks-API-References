---
title: "Timescale"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Définit les options qui spécifient comment rendre l'échelle de temps dans les vues Utilisation des tâches du diagramme de Gantt ou Utilisation des ressources lorsqu'un projet est exporté vers un format graphique."
type: docs
weight: 323
url: /fr/java/com.aspose.tasks/timescale/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.ValueType, com.aspose.ms.System.Enum
```
public final class Timescale extends System.Enum
```

Définit les options qui spécifient comment rendre l'échelle de temps dans les vues Diagramme de Gantt, Utilisation des tâches ou Utilisation des ressources lorsque le projet est exporté vers un format graphique.
## Champs

| Champ | Description |
| --- | --- |
| [Days](#Days) | Échelle de temps à deux niveaux prédéfinie où le niveau de détail minimal est d'un jour. |
| [DefinedInView](#DefinedInView) | Utilisez les paramètres d'échelle de temps définis dans les propriétés de la vue du projet : `GanttChartView.BottomTimescaleTier`([GanttChartView.getBottomTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getBottomTimescaleTier--)/[GanttChartView.setBottomTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setBottomTimescaleTier-TimescaleTier-)), `GanttChartView.MiddleTimescaleTier`([GanttChartView.getMiddleTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getMiddleTimescaleTier--)/[GanttChartView.setMiddleTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setMiddleTimescaleTier-TimescaleTier-)), `GanttChartView.TopTimescaleTier`([GanttChartView.getTopTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getTopTimescaleTier--)/[GanttChartView.setTopTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setTopTimescaleTier-TimescaleTier-)). |
| [Months](#Months) | Échelle de temps à deux niveaux prédéfinie où le niveau de détail minimal est d'un mois. |
| [ThirdsOfMonths](#ThirdsOfMonths) | Échelle de temps à deux niveaux prédéfinie où le niveau de détail est un tiers du mois. |
### Days {#Days}
```
public static final int Days
```


Échelle de temps à deux niveaux prédéfinie où le niveau de détail minimal est d'un jour.

### DefinedInView {#DefinedInView}
```
public static final int DefinedInView
```


Utilisez les paramètres d'échelle de temps définis dans les propriétés de la vue du projet : `GanttChartView.BottomTimescaleTier`([GanttChartView.getBottomTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getBottomTimescaleTier--)/[GanttChartView.setBottomTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setBottomTimescaleTier-TimescaleTier-)), `GanttChartView.MiddleTimescaleTier`([GanttChartView.getMiddleTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getMiddleTimescaleTier--)/[GanttChartView.setMiddleTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setMiddleTimescaleTier-TimescaleTier-)), `GanttChartView.TopTimescaleTier`([GanttChartView.getTopTimescaleTier()](../../com.aspose.tasks/ganttchartview\#getTopTimescaleTier--)/[GanttChartView.setTopTimescaleTier(TimescaleTier)](../../com.aspose.tasks/ganttchartview\#setTopTimescaleTier-TimescaleTier-)). Valide pour les formats contenant des données de vue. Par exemple, les projets lus au format MPP.

--------------------

Si les paramètres d'échelle de temps ne sont pas définis pour la vue, le paramètre prédéfini Timescale.Days est utilisé à la place.

### Months {#Months}
```
public static final int Months
```


Échelle de temps à deux niveaux prédéfinie où le niveau de détail minimal est d'un mois.

### ThirdsOfMonths {#ThirdsOfMonths}
```
public static final int ThirdsOfMonths
```


Échelle de temps à deux niveaux prédéfinie où le niveau de détail est un tiers du mois.

