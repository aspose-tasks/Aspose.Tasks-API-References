---
title: "GanttChartView"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente une vue GanttChart."
type: docs
weight: 112
url: /fr/java/com.aspose.tasks/ganttchartview/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.View](../../com.aspose.tasks/view)

**All Implemented Interfaces:**
com.aspose.tasks.ITimescaledView
```
public class GanttChartView extends View implements ITimescaledView
```

Représente une vue GanttChart.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [GanttChartView()](#GanttChartView--) | Initialise une nouvelle instance de la classe [GanttChartView](../../com.aspose.tasks/ganttchartview). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getAutoFilters()](#getAutoFilters--) | Obtient une liste de filtres automatiques d’une vue Gantt Chart. |
| [getBarRounding()](#getBarRounding--) | Obtient une valeur indiquant si les barres sont arrondies au jour le plus proche. |
| [getBarSize()](#getBarSize--) | Obtient la hauteur, en points, des barres Gantt dans le diagramme Gantt. |
| [getBarStyles()](#getBarStyles--) | Obtient une liste des styles de barres parents (communs) de la vue Gantt Chart. |
| [getBottomTimescaleTier()](#getBottomTimescaleTier--) | Obtient les paramètres du niveau inférieur de l'échelle de temps de la vue. |
| [getCustomBarStyles()](#getCustomBarStyles--) | Obtient une liste des styles de barres personnalisés spécifiques aux tâches de la vue Gantt Chart. |
| [getGridlines()](#getGridlines--) | Obtient une liste de `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) de la vue Gantt Chart. |
| [getHideRollupBarsWhenSummaryExpanded()](#getHideRollupBarsWhenSummaryExpanded--) | Obtient une valeur indiquant si les barres de regroupement seront masquées lors de l'expansion de la tâche récapitulative. |
| [getMiddleTimescaleTier()](#getMiddleTimescaleTier--) | Obtient les paramètres du niveau intermédiaire de l'échelle de temps de la vue. |
| [getNonWorkingTimeColor()](#getNonWorkingTimeColor--) | Obtient la couleur du temps non travaillé. |
| [getProgressLines()](#getProgressLines--) | Obtient les lignes de progression pour la vue Gantt Chart. |
| [getRollUpGanttBars()](#getRollUpGanttBars--) | Obtient une valeur indiquant si les barres du diagramme Gantt doivent être regroupées. |
| [getShowBarSplits()](#getShowBarSplits--) | Obtient une valeur indiquant si les découpes de tâches sur le diagramme Gantt doivent être affichées. |
| [getShowDrawings()](#getShowDrawings--) | Obtient une valeur indiquant si les dessins sur le diagramme Gantt doivent être affichés. |
| [getTableTextStyles()](#getTableTextStyles--) | Obtient une liste des styles de texte de tableau de la vue Gantt Chart. |
| [getTextStyles()](#getTextStyles--) | Obtient une liste de [TextStyle](../../com.aspose.tasks/textstyle) de la vue Gantt Chart. |
| [getTimescaleSizePercentage()](#getTimescaleSizePercentage--) | \{@inheritDoc\} |
| [getTopTimescaleTier()](#getTopTimescaleTier--) | Obtient les paramètres du niveau supérieur de l'échelle de temps de la vue. |
| [setBarRounding(boolean value)](#setBarRounding-boolean-) | Définit une valeur indiquant si les barres sont arrondies au jour le plus proche. |
| [setBarSize(int value)](#setBarSize-int-) | Définit la hauteur, en points, des barres Gantt dans le diagramme Gantt. |
| [setBottomTimescaleTier(TimescaleTier value)](#setBottomTimescaleTier-com.aspose.tasks.TimescaleTier-) | Définit les paramètres du niveau inférieur de l'échelle de temps de la vue. |
| [setGridlines(List&lt;Gridlines&gt; value)](#setGridlines-java.util.List-com.aspose.tasks.Gridlines--) | Définit une liste de `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) de la vue du diagramme de Gantt. |
| [setHideRollupBarsWhenSummaryExpanded(boolean value)](#setHideRollupBarsWhenSummaryExpanded-boolean-) | Définit une valeur indiquant si les barres de regroupement seront masquées lors de l'expansion de la tâche récapitulative. |
| [setMiddleTimescaleTier(TimescaleTier value)](#setMiddleTimescaleTier-com.aspose.tasks.TimescaleTier-) | Définit les paramètres du niveau d’échelle de temps moyen de la vue. |
| [setNonWorkingTimeColor(Color value)](#setNonWorkingTimeColor-java.awt.Color-) | Définit la couleur du temps non travaillé. |
| [setProgressLines(ProgressLines value)](#setProgressLines-com.aspose.tasks.ProgressLines-) | Définit les lignes de progression pour la vue du diagramme de Gantt. |
| [setRollUpGanttBars(boolean value)](#setRollUpGanttBars-boolean-) | Définit une valeur indiquant si les barres du diagramme de Gantt doivent être regroupées. |
| [setShowBarSplits(boolean value)](#setShowBarSplits-boolean-) | Définit une valeur indiquant si les découpages de tâches sur le diagramme de Gantt doivent être affichés. |
| [setShowDrawings(boolean value)](#setShowDrawings-boolean-) | Définit une valeur indiquant si les dessins sur le diagramme de Gantt doivent être affichés. |
| [setTextStyles(List&lt;TextStyle&gt; value)](#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--) | Définit une liste de [TextStyle](../../com.aspose.tasks/textstyle) de la vue du diagramme de Gantt. |
| [setTimescaleSizePercentage(int value)](#setTimescaleSizePercentage-int-) | \{@inheritDoc\} |
| [setTopTimescaleTier(TimescaleTier value)](#setTopTimescaleTier-com.aspose.tasks.TimescaleTier-) | Définit les paramètres du niveau d'échelle de temps supérieur de la vue. |
### GanttChartView() {#GanttChartView--}
```
public GanttChartView()
```


Initialise une nouvelle instance de la classe [GanttChartView](../../com.aspose.tasks/ganttchartview).

### getAutoFilters() {#getAutoFilters--}
```
public final FilterCollection getAutoFilters()
```


Obtient une liste de filtres automatiques d’une vue Gantt Chart.

**Returns:**
[FilterCollection](../../com.aspose.tasks/filtercollection) - a list of auto filters of a Gantt Chart view.
### getBarRounding() {#getBarRounding--}
```
public final boolean getBarRounding()
```


Obtient une valeur indiquant si les barres sont arrondies au jour le plus proche. La valeur par défaut est True.

**Returns:**
boolean - une valeur indiquant si les barres sont arrondies au jour le plus proche.
### getBarSize() {#getBarSize--}
```
public final int getBarSize()
```


Obtient la hauteur, en points, des barres Gantt dans le diagramme Gantt.

**Returns:**
int - la hauteur, en points, des barres Gantt dans le diagramme de Gantt.
### getBarStyles() {#getBarStyles--}
```
public final List<GanttBarStyle> getBarStyles()
```


Obtient une liste des styles de barres parents (communs) de la vue du diagramme de Gantt. [GanttBarStyle](../../com.aspose.tasks/ganttbarstyle).

**Returns:**
java.util.List&lt;com.aspose.tasks.GanttBarStyle&gt; - une liste des styles de barres parents (communs) de la vue du diagramme de Gantt.
### getBottomTimescaleTier() {#getBottomTimescaleTier--}
```
public final TimescaleTier getBottomTimescaleTier()
```


Obtient les paramètres du niveau d'échelle de temps inférieur de la vue. [TimescaleTier](../../com.aspose.tasks/timescaletier)

**Returns:**
[TimescaleTier](../../com.aspose.tasks/timescaletier) - settings of view's bottom timescale tier.
### getCustomBarStyles() {#getCustomBarStyles--}
```
public final List<GanttBarStyle> getCustomBarStyles()
```


Obtient une liste des styles de barres personnalisés spécifiques aux tâches de la vue du diagramme de Gantt. [GanttBarStyle](../../com.aspose.tasks/ganttbarstyle).

**Returns:**
java.util.List&lt;com.aspose.tasks.GanttBarStyle&gt; - une liste des styles de barres personnalisés spécifiques aux tâches de la vue du diagramme de Gantt.
### getGridlines() {#getGridlines--}
```
public final List<Gridlines> getGridlines()
```


Obtient une liste de `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) de la vue Gantt Chart.

**Returns:**
java.util.List&lt;com.aspose.tasks.Gridlines&gt; - une liste de `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) de la vue du diagramme de Gantt.
### getHideRollupBarsWhenSummaryExpanded() {#getHideRollupBarsWhenSummaryExpanded--}
```
public final boolean getHideRollupBarsWhenSummaryExpanded()
```


Obtient une valeur indiquant si les barres de regroupement seront masquées lors de l'expansion de la tâche récapitulative.

**Returns:**
boolean - une valeur indiquant si les barres de regroupement seront masquées lors de l'expansion de la tâche récapitulative.
### getMiddleTimescaleTier() {#getMiddleTimescaleTier--}
```
public final TimescaleTier getMiddleTimescaleTier()
```


Obtient les paramètres du niveau d'échelle de temps moyen de la vue. [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Returns:**
[TimescaleTier](../../com.aspose.tasks/timescaletier) - settings of view's middle timescale tier.
### getNonWorkingTimeColor() {#getNonWorkingTimeColor--}
```
public final Color getNonWorkingTimeColor()
```


Obtient la couleur du temps non travaillé.

**Returns:**
java.awt.Color - couleur du temps non travaillé.
### getProgressLines() {#getProgressLines--}
```
public final ProgressLines getProgressLines()
```


Obtient les lignes de progression pour la vue du diagramme de Gantt. `ProgressLines`([getProgressLines()](../../com.aspose.tasks/ganttchartview\#getProgressLines--)/[setProgressLines(ProgressLines)](../../com.aspose.tasks/ganttchartview\#setProgressLines-ProgressLines-)).

**Returns:**
[ProgressLines](../../com.aspose.tasks/progresslines) - progress lines for the Gantt Chart view.
### getRollUpGanttBars() {#getRollUpGanttBars--}
```
public final boolean getRollUpGanttBars()
```


Obtient une valeur indiquant si les barres du diagramme Gantt doivent être regroupées.

**Returns:**
boolean - une valeur indiquant si les barres du diagramme de Gantt doivent être regroupées.
### getShowBarSplits() {#getShowBarSplits--}
```
public final boolean getShowBarSplits()
```


Obtient une valeur indiquant si les découpes de tâches sur le diagramme Gantt doivent être affichées.

**Returns:**
boolean - une valeur indiquant si les découpages de tâches sur le diagramme de Gantt doivent être affichés.
### getShowDrawings() {#getShowDrawings--}
```
public final boolean getShowDrawings()
```


Obtient une valeur indiquant si les dessins sur le diagramme Gantt doivent être affichés.

**Returns:**
boolean - une valeur indiquant si les dessins sur le diagramme de Gantt doivent être affichés.
### getTableTextStyles() {#getTableTextStyles--}
```
public final List<TableTextStyle> getTableTextStyles()
```


Obtient une liste des styles de texte de tableau de la vue du diagramme de Gantt. [TableTextStyle](../../com.aspose.tasks/tabletextstyle).

**Returns:**
java.util.List&lt;com.aspose.tasks.TableTextStyle&gt; - une liste des styles de texte de tableau de la vue du diagramme de Gantt.
### getTextStyles() {#getTextStyles--}
```
public final List<TextStyle> getTextStyles()
```


Obtient une liste de [TextStyle](../../com.aspose.tasks/textstyle) de la vue Gantt Chart.

**Returns:**
java.util.List&lt;com.aspose.tasks.TextStyle&gt; - une liste de [TextStyle](../../com.aspose.tasks/textstyle) de la vue du diagramme de Gantt.
### getTimescaleSizePercentage() {#getTimescaleSizePercentage--}
```
public final int getTimescaleSizePercentage()
```


Obtient un pourcentage pour réduire ou agrandir l'espacement entre les unités sur le niveau d'échelle de temps.

**Returns:**
int - \{@inheritDoc\}
### getTopTimescaleTier() {#getTopTimescaleTier--}
```
public final TimescaleTier getTopTimescaleTier()
```


Obtient les paramètres du niveau d'échelle de temps supérieur de la vue. [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Returns:**
[TimescaleTier](../../com.aspose.tasks/timescaletier) - settings of view's top timescale tier.
### setBarRounding(boolean value) {#setBarRounding-boolean-}
```
public final void setBarRounding(boolean value)
```


Définit une valeur indiquant si les barres sont arrondies au jour le plus proche. La valeur par défaut est True.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant si les barres sont arrondies au jour le plus proche. |

### setBarSize(int value) {#setBarSize-int-}
```
public final void setBarSize(int value)
```


Définit la hauteur, en points, des barres Gantt dans le diagramme Gantt.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | la hauteur, en points, des barres Gantt dans le diagramme de Gantt. |

### setBottomTimescaleTier(TimescaleTier value) {#setBottomTimescaleTier-com.aspose.tasks.TimescaleTier-}
```
public final void setBottomTimescaleTier(TimescaleTier value)
```


Définit les paramètres du niveau d'échelle de temps inférieur de la vue. [TimescaleTier](../../com.aspose.tasks/timescaletier)

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [TimescaleTier](../../com.aspose.tasks/timescaletier) | paramètres du niveau d'échelle de temps inférieur de la vue. |

### setGridlines(List&lt;Gridlines&gt; value) {#setGridlines-java.util.List-com.aspose.tasks.Gridlines--}
```
public final void setGridlines(List<Gridlines> value)
```


Définit une liste de `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) de la vue du diagramme de Gantt.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.Gridlines&gt; | une liste de `Gridlines`([getGridlines()](../../com.aspose.tasks/ganttchartview\#getGridlines--)/[setGridlines(java.util.List)](../../com.aspose.tasks/ganttchartview\#setGridlines-java.util.List-Gridlines--)) de la vue du diagramme de Gantt. |

### setHideRollupBarsWhenSummaryExpanded(boolean value) {#setHideRollupBarsWhenSummaryExpanded-boolean-}
```
public final void setHideRollupBarsWhenSummaryExpanded(boolean value)
```


Définit une valeur indiquant si les barres de regroupement seront masquées lors de l'expansion de la tâche récapitulative.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant si les barres de regroupement seront masquées lors de l'expansion de la tâche récapitulative. |

### setMiddleTimescaleTier(TimescaleTier value) {#setMiddleTimescaleTier-com.aspose.tasks.TimescaleTier-}
```
public final void setMiddleTimescaleTier(TimescaleTier value)
```


Définit les paramètres du niveau d'échelle de temps moyen de la vue. [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [TimescaleTier](../../com.aspose.tasks/timescaletier) | paramètres du niveau d'échelle de temps moyen de la vue. |

### setNonWorkingTimeColor(Color value) {#setNonWorkingTimeColor-java.awt.Color-}
```
public final void setNonWorkingTimeColor(Color value)
```


Définit la couleur du temps non travaillé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.awt.Color | couleur du temps non travaillé. |

### setProgressLines(ProgressLines value) {#setProgressLines-com.aspose.tasks.ProgressLines-}
```
public final void setProgressLines(ProgressLines value)
```


Définit les lignes de progression pour la vue du diagramme de Gantt. `ProgressLines`([getProgressLines()](../../com.aspose.tasks/ganttchartview\#getProgressLines--)/[setProgressLines(ProgressLines)](../../com.aspose.tasks/ganttchartview\#setProgressLines-ProgressLines-)).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [ProgressLines](../../com.aspose.tasks/progresslines) | lignes de progression pour la vue du diagramme de Gantt. |

### setRollUpGanttBars(boolean value) {#setRollUpGanttBars-boolean-}
```
public final void setRollUpGanttBars(boolean value)
```


Définit une valeur indiquant si les barres du diagramme de Gantt doivent être regroupées.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant si les barres du diagramme de Gantt doivent être regroupées. |

### setShowBarSplits(boolean value) {#setShowBarSplits-boolean-}
```
public final void setShowBarSplits(boolean value)
```


Définit une valeur indiquant si les découpages de tâches sur le diagramme de Gantt doivent être affichés.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant si les divisions de tâche sur le diagramme de Gantt doivent être affichées. |

### setShowDrawings(boolean value) {#setShowDrawings-boolean-}
```
public final void setShowDrawings(boolean value)
```


Définit une valeur indiquant si les dessins sur le diagramme de Gantt doivent être affichés.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant si les dessins sur le diagramme de Gantt doivent être affichés. |

### setTextStyles(List&lt;TextStyle&gt; value) {#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--}
```
public final void setTextStyles(List<TextStyle> value)
```


Définit une liste de [TextStyle](../../com.aspose.tasks/textstyle) de la vue du diagramme de Gantt.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.TextStyle&gt; | une liste de [TextStyle](../../com.aspose.tasks/textstyle) de la vue du diagramme de Gantt. |

### setTimescaleSizePercentage(int value) {#setTimescaleSizePercentage-int-}
```
public final void setTimescaleSizePercentage(int value)
```


Définit un pourcentage pour réduire ou agrandir l'espacement entre les unités sur le niveau d'échelle de temps.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | \{@inheritDoc\} |

### setTopTimescaleTier(TimescaleTier value) {#setTopTimescaleTier-com.aspose.tasks.TimescaleTier-}
```
public final void setTopTimescaleTier(TimescaleTier value)
```


Définit les paramètres du niveau d'échelle de temps supérieur de la vue. [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [TimescaleTier](../../com.aspose.tasks/timescaletier) | paramètres du niveau d'échelle de temps supérieur de la vue. |

