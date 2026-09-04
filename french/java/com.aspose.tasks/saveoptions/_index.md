---
title: "SaveOptions"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Ceci est une classe de base abstraite pour les classes qui permettent à l'utilisateur de spécifier des options supplémentaires lors de l'enregistrement d'un projet dans un format particulier."
type: docs
weight: 274
url: /fr/java/com.aspose.tasks/saveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public abstract class SaveOptions extends SimpleSaveOptions
```

Ceci est une classe de base abstraite pour les classes qui permettent à l'utilisateur de spécifier des options supplémentaires lors de l'enregistrement d'un projet dans un format particulier.

--------------------

Une instance de toute classe dérivée de la classe SaveOptions est transmise aux surcharges Save de flux ou Save de chaîne afin que l'utilisateur définisse des options personnalisées lors de l'enregistrement d'un document.
## Méthodes

| Méthode | Description |
| --- | --- |
| [getBarStyles()](#getBarStyles--) | Obtient la liste des instances de la classe [BarStyle](../../com.aspose.tasks/barstyle) qui apparaissent dans la vue du projet. |
| [getCustomPageSize()](#getCustomPageSize--) | Obtient la taille de page personnalisée en points (1 point = 1/72 de pouce). |
| [getDrawNonWorkingTime()](#getDrawNonWorkingTime--) | Obtient une valeur indiquant si le temps non travaillé doit être affiché (la valeur par défaut est TRUE). |
| [getEndDate()](#getEndDate--) | Obtient une date jusqu'à laquelle le rendu doit se terminer. |
| [getFitContent()](#getFitContent--) | Obtient une valeur indiquant si la hauteur de la ligne doit être augmentée pour s'adapter à son contenu. |
| [getGridlines()](#getGridlines--) | Obtient une liste de [Gridline](../../com.aspose.tasks/gridline) qui apparaissent dans la vue du projet. |
| [getLegendDrawingOptions()](#getLegendDrawingOptions--) | Obtient une valeur qui définit comment rendre une légende. |
| [getLegendItems()](#getLegendItems--) | Obtient un tableau de PageLegendItem qui définit quelles barres doivent être rendues dans la légende de la page. |
| [getMarkCriticalTasks()](#getMarkCriticalTasks--) | Obtient une valeur indiquant si les tâches critiques doivent être affichées en rouge (la valeur par défaut est FALSE). |
| [getNonWorkingTimeColor()](#getNonWorkingTimeColor--) | Obtient la couleur du temps non travaillé. |
| [getPageCount()](#getPageCount--) | Obtient le nombre de pages du projet. |
| [getPageSize()](#getPageSize--) | Obtient la taille de la page à rendre (la valeur par défaut est PageSize.A4). |
| [getPresentationFormat()](#getPresentationFormat--) | Obtient le `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) dans lequel le document sera enregistré. |
| [getRenderToSinglePage()](#getRenderToSinglePage--) | Obtient une valeur indiquant si un projet doit être rendu sur une seule page lorsque le projet est enregistré au format graphique. |
| [getRollUpGanttBars()](#getRollUpGanttBars--) | Obtient une valeur indiquant si les sous‑tâches sur la barre de tâche récapitulative doivent être marquées. |
| [getStartDate()](#getStartDate--) | Obtient la date à partir de laquelle commencer le rendu. |
| [getTaskLinkDrawingCallback()](#getTaskLinkDrawingCallback--) | Obtient un callback qui peut être utilisé pour personnaliser certains aspects du rendu des liens de tâches. |
| [getTextStyles()](#getTextStyles--) | Obtient la liste des styles de texte appliqués lors du rendu d’une vue de projet. |
| [getTimescale()](#getTimescale--) | Obtient la valeur `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) qui est utilisée pour contrôler la façon dont l’échelle de temps (si présente) est rendue lorsque le projet est enregistré au format graphique. |
| [getTimescaleFitBehavior()](#getTimescaleFitBehavior--) | Obtient un comportement qui définit comment aligner l’extrémité droite de l’échelle de temps avec la fin de la page. |
| [getUseGradientBrush()](#getUseGradientBrush--) | Obtient une valeur indiquant si un pinceau dégradé doit être utilisé lors du rendu du diagramme de Gantt. |
| [getView()](#getView--) | Obtient la liste des colonnes de vue à rendre ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). |
| [getViewSettings()](#getViewSettings--) | Obtient une vue (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) à rendre. |
| [isPortrait()](#isPortrait--) | Obtient une valeur indiquant si l'orientation de la page est portrait ; renvoie false si l'orientation de la page est paysage. |
| [setBarStyles(List&lt;BarStyle&gt; value)](#setBarStyles-java.util.List-com.aspose.tasks.BarStyle--) | Définit la liste des instances de la classe [BarStyle](../../com.aspose.tasks/barstyle) qui apparaissent dans la vue du projet. |
| [setCustomPageSize(Dimension2D value)](#setCustomPageSize-java.awt.geom.Dimension2D-) | Définit la taille de page personnalisée en points (1 point = 1/72 de pouce). |
| [setDrawNonWorkingTime(boolean value)](#setDrawNonWorkingTime-boolean-) | Définit une valeur indiquant si le temps non travaillé doit être dessiné (la valeur par défaut est TRUE). |
| [setEndDate(Date value)](#setEndDate-java.util.Date-) | Définit une date jusqu’à laquelle terminer le rendu. |
| [setFitContent(boolean value)](#setFitContent-boolean-) | Définit une valeur indiquant si la hauteur de la ligne doit être augmentée pour s’adapter à son contenu. |
| [setGridlines(List&lt;Gridline&gt; value)](#setGridlines-java.util.List-com.aspose.tasks.Gridline--) | Définit une liste de [Gridline](../../com.aspose.tasks/gridline) qui apparaissent dans la vue du projet. |
| [setLegendDrawingOptions(int value)](#setLegendDrawingOptions-int-) | Définit une valeur qui définit comment rendre une légende. |
| [setLegendItems(PageLegendItem[] value)](#setLegendItems-com.aspose.tasks.PageLegendItem---) | Définit un tableau de PageLegendItem qui définit quelles barres doivent être rendues dans la légende de la page. |
| [setMarkCriticalTasks(boolean value)](#setMarkCriticalTasks-boolean-) | Définit une valeur indiquant si les tâches critiques doivent être affichées en rouge (la valeur par défaut est FALSE). |
| [setNonWorkingTimeColor(Color value)](#setNonWorkingTimeColor-java.awt.Color-) | Définit la couleur du temps non travaillé. |
| [setPageSize(int value)](#setPageSize-int-) | Définit la taille de la page à rendre (la valeur par défaut est PageSize.A4). |
| [setPortrait(boolean value)](#setPortrait-boolean-) | Définit une valeur indiquant si l'orientation de la page est portrait ; renvoie false si l'orientation de la page est paysage. |
| [setPresentationFormat(int value)](#setPresentationFormat-int-) | Définit le `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) dans lequel le document sera enregistré. |
| [setRenderToSinglePage(boolean value)](#setRenderToSinglePage-boolean-) | Définit une valeur indiquant si un projet doit être rendu sur une seule page lorsque le projet est enregistré au format graphique. |
| [setRollUpGanttBars(boolean value)](#setRollUpGanttBars-boolean-) | Définit une valeur indiquant si les sous‑tâches sur la barre de tâche récapitulative doivent être marquées. |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | Définit la date à partir de laquelle le rendu commence. |
| [setTaskLinkDrawingCallback(TaskLinkDrawingCallbackDelegate value)](#setTaskLinkDrawingCallback-com.aspose.tasks.TaskLinkDrawingCallbackDelegate-) | Définit un rappel qui peut être utilisé pour personnaliser certains aspects du rendu des liens de tâches. |
| [setTextStyles(List&lt;TextStyle&gt; value)](#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--) | Définit la liste des styles de texte appliqués lors du rendu d'une vue de projet. |
| [setTimescale(int value)](#setTimescale-int-) | Définit la valeur `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) qui est utilisée pour contrôler la façon dont l'échelle de temps (si présente) est rendue lorsque le projet est enregistré au format graphique. |
| [setTimescaleFitBehavior(int value)](#setTimescaleFitBehavior-int-) | Définit un comportement qui définit comment aligner l'extrémité droite de l'échelle de temps avec la fin de la page. |
| [setUseGradientBrush(boolean value)](#setUseGradientBrush-boolean-) | Définit une valeur indiquant si un pinceau dégradé doit être utilisé lors du rendu du diagramme de Gantt. |
| [setView(ProjectView value)](#setView-com.aspose.tasks.ProjectView-) | Définit une liste des colonnes de vue à rendre ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). |
| [setViewSettings(View value)](#setViewSettings-com.aspose.tasks.View-) | Définit une vue (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) à rendre. |
### getBarStyles() {#getBarStyles--}
```
public final List<BarStyle> getBarStyles()
```


Obtient la liste des instances de la classe [BarStyle](../../com.aspose.tasks/barstyle) qui apparaissent dans la vue du projet.

**Returns:**
java.util.List&lt;com.aspose.tasks.BarStyle&gt; - la liste des instances de la classe [BarStyle](../../com.aspose.tasks/barstyle) qui apparaissent dans la vue du projet.
### getCustomPageSize() {#getCustomPageSize--}
```
public final Dimension2D getCustomPageSize()
```


Obtient la taille de page personnalisée en points (1 point = 1/72 de pouce).

**Returns:**
java.awt.geom.Dimension2D - la taille de page personnalisée en points (1 point = 1/72 de pouce).
### getDrawNonWorkingTime() {#getDrawNonWorkingTime--}
```
public final boolean getDrawNonWorkingTime()
```


Obtient une valeur indiquant si le temps non travaillé doit être affiché (la valeur par défaut est TRUE).

**Returns:**
boolean - une valeur indiquant si le temps non travaillé doit être dessiné (La valeur par défaut est TRUE).
### getEndDate() {#getEndDate--}
```
public final Date getEndDate()
```


Obtient une date jusqu'à laquelle le rendu doit se terminer.

**Returns:**
java.util.Date - une date jusqu'à laquelle terminer le rendu.
### getFitContent() {#getFitContent--}
```
public final boolean getFitContent()
```


Obtient une valeur indiquant si la hauteur de la ligne doit être augmentée pour s'adapter à son contenu.

**Returns:**
boolean - une valeur indiquant si la hauteur de la ligne doit être augmentée pour s'adapter à son contenu.
### getGridlines() {#getGridlines--}
```
public final List<Gridline> getGridlines()
```


Obtient une liste de [Gridline](../../com.aspose.tasks/gridline) qui apparaissent dans la vue du projet.

**Returns:**
java.util.List&lt;com.aspose.tasks.Gridline&gt; - une liste de [Gridline](../../com.aspose.tasks/gridline) qui apparaissent dans la vue du projet.
### getLegendDrawingOptions() {#getLegendDrawingOptions--}
```
public final int getLegendDrawingOptions()
```


Obtient une valeur qui définit comment rendre une légende. La valeur par défaut est LegendDrawingOptions.OnEveryPage.

S'applique uniquement lorsque la vue du diagramme de Gantt est rendue.

**Returns:**
int - une valeur qui définit comment rendre une légende.
### getLegendItems() {#getLegendItems--}
```
public final PageLegendItem[] getLegendItems()
```


Obtient un tableau de PageLegendItem qui définit quelles barres doivent être rendues dans la légende de la page. Si null, les éléments par défaut sont rendus.

S'applique uniquement lorsque la vue du diagramme de Gantt est rendue.

**Returns:**
com.aspose.tasks.PageLegendItem[] - un tableau de PageLegendItem qui définit quelles barres doivent être rendues dans la légende de la page.
### getMarkCriticalTasks() {#getMarkCriticalTasks--}
```
public final boolean getMarkCriticalTasks()
```


Obtient une valeur indiquant si les tâches critiques doivent être affichées en rouge (la valeur par défaut est FALSE).

**Returns:**
boolean - une valeur indiquant si les tâches critiques doivent être affichées en couleur rouge (La valeur par défaut est FALSE).
### getNonWorkingTimeColor() {#getNonWorkingTimeColor--}
```
public final Color getNonWorkingTimeColor()
```


Obtient la couleur du temps non travaillé.

**Returns:**
java.awt.Color - la couleur du temps non travaillé.
### getPageCount() {#getPageCount--}
```
public final int getPageCount()
```


Obtient le nombre de pages du projet.

**Returns:**
int - le nombre de pages du projet.
### getPageSize() {#getPageSize--}
```
public final int getPageSize()
```


Obtient la taille de la page à rendre (la valeur par défaut est PageSize.A4).

**Returns:**
int - la taille de la page à rendre (La valeur par défaut est PageSize.A4).
### getPresentationFormat() {#getPresentationFormat--}
```
public final int getPresentationFormat()
```


Obtient le `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) dans lequel le document sera enregistré.

**Returns:**
int - le `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) dans lequel le document sera enregistré.
### getRenderToSinglePage() {#getRenderToSinglePage--}
```
public final boolean getRenderToSinglePage()
```


Obtient une valeur indiquant si un projet doit être rendu sur une seule page lorsque le projet est enregistré au format graphique. La taille de la page sera modifiée afin que le projet rendu puisse tenir sur une page.

**Returns:**
boolean - une valeur indiquant si un projet doit être rendu sur une seule page lorsque le projet est enregistré au format graphique.
### getRollUpGanttBars() {#getRollUpGanttBars--}
```
public final boolean getRollUpGanttBars()
```


Obtient une valeur indiquant si les sous‑tâches sur la barre de tâche récapitulative doivent être marquées. Pour les sous‑tâches, le champ Rollup indique si les informations des barres Gantt de la sous‑tâche seront agrégées vers la barre de tâche récapitulative. Pour les tâches récapitulatives, le champ Rollup indique si la barre de tâche récapitulative affiche les barres agrégées. Vous devez définir le champ Rollup des tâches récapitulatives sur Oui pour que les sous‑tâches puissent être agrégées.

--------------------

S'applique uniquement lorsque la vue du diagramme de Gantt est rendue.

**Returns:**
boolean - une valeur indiquant si les sous‑tâches sur la barre de tâche récapitulative doivent être marquées.
### getStartDate() {#getStartDate--}
```
public final Date getStartDate()
```


Obtient la date à partir de laquelle commencer le rendu.

**Returns:**
java.util.Date - la date à partir de laquelle commencer le rendu.
### getTaskLinkDrawingCallback() {#getTaskLinkDrawingCallback--}
```
public final TaskLinkDrawingCallbackDelegate getTaskLinkDrawingCallback()
```


Obtient un callback qui peut être utilisé pour personnaliser certains aspects du rendu des liens de tâches.

S'applique uniquement lorsque la vue du diagramme de Gantt est rendue.

**Returns:**
[TaskLinkDrawingCallbackDelegate](../../com.aspose.tasks/tasklinkdrawingcallbackdelegate) - a callback that can be used to customize some aspects of task links rendering.
### getTextStyles() {#getTextStyles--}
```
public final List<TextStyle> getTextStyles()
```


Obtient la liste des styles de texte appliqués lors du rendu d’une vue de projet.

--------------------

Ces styles remplacent les styles définis avec GanttCharView.setTextStyles.

**Returns:**
java.util.List&lt;com.aspose.tasks.TextStyle&gt; - la liste des styles de texte appliqués lors du rendu d’une vue de projet.
### getTimescale() {#getTimescale--}
```
public final int getTimescale()
```


Obtient la valeur `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) qui est utilisée pour contrôler la façon dont l’échelle de temps (si présente) est rendue lorsque le projet est enregistré au format graphique.

**Returns:**
int - la valeur `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) qui est utilisée pour contrôler la façon dont l’échelle de temps (si présente) est rendue lorsque le projet est enregistré au format graphique.
### getTimescaleFitBehavior() {#getTimescaleFitBehavior--}
```
public final int getTimescaleFitBehavior()
```


Obtient un comportement qui définit comment aligner l’extrémité droite de l’échelle de temps avec la fin de la page.

**Returns:**
int - un comportement qui définit comment aligner l’extrémité droite de l’échelle de temps avec la fin de la page.
### getUseGradientBrush() {#getUseGradientBrush--}
```
public boolean getUseGradientBrush()
```


Obtient une valeur indiquant si un pinceau dégradé doit être utilisé lors du rendu du diagramme de Gantt.

--------------------

S'applique uniquement lorsque la vue du diagramme de Gantt est rendue.

**Returns:**
boolean - une valeur indiquant si un pinceau dégradé doit être utilisé lors du rendu du diagramme de Gantt.
### getView() {#getView--}
```
public final ProjectView getView()
```


Obtient une liste des colonnes de vue à rendre ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). Si non définies, seuls les identifiants de tâche, les noms de tâche, le début et la fin sont rendus. Si les propriétés View et `ViewSettings`([getViewSettings()](../../com.aspose.tasks/saveoptions\#getViewSettings--)/[setViewSettings(View)](../../com.aspose.tasks/saveoptions\#setViewSettings-View-)) sont toutes deux définies, les colonnes provenant de View remplacent celles de ViewSettings.

**Returns:**
[ProjectView](../../com.aspose.tasks/projectview) - a list of the view columns to render ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)).
### getViewSettings() {#getViewSettings--}
```
public final View getViewSettings()
```


Obtient une vue (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) à rendre. Vous pouvez utiliser cette option pour spécifier explicitement quelle vue doit être enregistrée aux formats PDF, HTML ou Image. Si cette propriété est définie, la propriété [PresentationFormat](../../com.aspose.tasks/presentationformat) est ignorée lors de l’enregistrement du projet. La vue doit provenir de l’un des écrans suivants ((`Aspose.Tasks.View.Screen`([View.getScreen()](../../com.aspose.tasks/view\#getScreen--)/[View.setScreen(int)](../../com.aspose.tasks/view\#setScreen-int-)))) : (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage)

**Returns:**
[View](../../com.aspose.tasks/view) - a view (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) to render.
### isPortrait() {#isPortrait--}
```
public final boolean isPortrait()
```


Obtient une valeur indiquant si l'orientation de la page est portrait ; renvoie false si l'orientation de la page est paysage.

--------------------

Ne s’applique pas lorsque SaveOptions.getPageSize() == PageSize.DefinedInView. Dans ce cas, [PageSettings.isPortrait()](../../com.aspose.tasks/pagesettings\#isPortrait--) est utilisé à la place. Ne s’applique pas lorsque [getCustomPageSize()](../../com.aspose.tasks/saveoptions\#getCustomPageSize--) est défini.

**Returns:**
boolean - une valeur indiquant si l'orientation de la page est portrait ; renvoie false si l'orientation de la page est paysage.
### setBarStyles(List&lt;BarStyle&gt; value) {#setBarStyles-java.util.List-com.aspose.tasks.BarStyle--}
```
public final void setBarStyles(List<BarStyle> value)
```


Définit la liste des instances de la classe [BarStyle](../../com.aspose.tasks/barstyle) qui apparaissent dans la vue du projet.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.BarStyle&gt; | la liste des instances de la classe [BarStyle](../../com.aspose.tasks/barstyle) qui apparaissent dans la vue du projet. |

### setCustomPageSize(Dimension2D value) {#setCustomPageSize-java.awt.geom.Dimension2D-}
```
public final void setCustomPageSize(Dimension2D value)
```


Définit la taille de page personnalisée en points (1 point = 1/72 de pouce).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.awt.geom.Dimension2D | la taille de page personnalisée en points (1 point = 1/72 de pouce). |

### setDrawNonWorkingTime(boolean value) {#setDrawNonWorkingTime-boolean-}
```
public final void setDrawNonWorkingTime(boolean value)
```


Définit une valeur indiquant si le temps non travaillé doit être dessiné (la valeur par défaut est TRUE).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant si le temps non travaillé doit être dessiné (la valeur par défaut est TRUE). |

### setEndDate(Date value) {#setEndDate-java.util.Date-}
```
public final void setEndDate(Date value)
```


Définit une date jusqu’à laquelle terminer le rendu.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.Date | une date jusqu’à laquelle terminer le rendu. |

### setFitContent(boolean value) {#setFitContent-boolean-}
```
public final void setFitContent(boolean value)
```


Définit une valeur indiquant si la hauteur de la ligne doit être augmentée pour s’adapter à son contenu.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant si la hauteur de ligne doit être augmentée pour s’adapter à son contenu. |

### setGridlines(List&lt;Gridline&gt; value) {#setGridlines-java.util.List-com.aspose.tasks.Gridline--}
```
public final void setGridlines(List<Gridline> value)
```


Définit une liste de [Gridline](../../com.aspose.tasks/gridline) qui apparaissent dans la vue du projet.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | java.util.List&lt;com.aspose.tasks.Gridline&gt; | une liste de [Gridline](../../com.aspose.tasks/gridline) qui apparaissent dans la vue du projet. |

### setLegendDrawingOptions(int value) {#setLegendDrawingOptions-int-}
```
public final void setLegendDrawingOptions(int value)
```


Définit une valeur qui définit comment rendre une légende. La valeur par défaut est LegendDrawingOptions.OnEveryPage.

S'applique uniquement lorsque la vue du diagramme de Gantt est rendue.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | une valeur qui définit comment rendre une légende. |

### setLegendItems(PageLegendItem[] value) {#setLegendItems-com.aspose.tasks.PageLegendItem---}
```
public final void setLegendItems(PageLegendItem[] value)
```


Définit un tableau de PageLegendItem qui indique quelles barres doivent être rendues dans la légende de page. Si null, les éléments par défaut sont rendus.

S'applique uniquement lorsque la vue du diagramme de Gantt est rendue.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [PageLegendItem\[\]](../../com.aspose.tasks/pagelegenditem) | un tableau de PageLegendItem qui indique quelles barres doivent être rendues dans la légende de page. |

### setMarkCriticalTasks(boolean value) {#setMarkCriticalTasks-boolean-}
```
public final void setMarkCriticalTasks(boolean value)
```


Définit une valeur indiquant si les tâches critiques doivent être affichées en rouge (la valeur par défaut est FALSE).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant si les tâches critiques doivent être affichées en couleur rouge (la valeur par défaut est FALSE). |

### setNonWorkingTimeColor(Color value) {#setNonWorkingTimeColor-java.awt.Color-}
```
public final void setNonWorkingTimeColor(Color value)
```


Définit la couleur du temps non travaillé.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.awt.Color | la couleur du temps non travaillé. |

### setPageSize(int value) {#setPageSize-int-}
```
public final void setPageSize(int value)
```


Définit la taille de la page à rendre (la valeur par défaut est PageSize.A4).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | la taille de la page à rendre (la valeur par défaut est PageSize.A4). |

### setPortrait(boolean value) {#setPortrait-boolean-}
```
public final void setPortrait(boolean value)
```


Définit une valeur indiquant si l'orientation de la page est portrait ; renvoie false si l'orientation de la page est paysage.

--------------------

Ne s'applique pas lorsque SaveOptions.PageSize == Visualization.PageSize.DefinedInView. Dans ce cas [PageSettings.setPortrait(boolean)](../../com.aspose/tasks/pagesettings\#setPortrait-boolean-) est utilisé à la place. Ne s'applique pas lorsque [getCustomPageSize()](../../com.aspose.tasks/saveoptions\#getCustomPageSize--) est défini.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant si l'orientation de la page est portrait ; renvoie false si l'orientation de la page est paysage. |

### setPresentationFormat(int value) {#setPresentationFormat-int-}
```
public final void setPresentationFormat(int value)
```


Définit le `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) dans lequel le document sera enregistré.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | int | le `PresentationFormat`([getPresentationFormat()](../../com.aspose.tasks/saveoptions\#getPresentationFormat--)/[setPresentationFormat(int)](../../com.aspose.tasks/saveoptions\#setPresentationFormat-int-)) dans lequel le document sera enregistré. |

### setRenderToSinglePage(boolean value) {#setRenderToSinglePage-boolean-}
```
public final void setRenderToSinglePage(boolean value)
```


Définit une valeur indiquant si un projet doit être rendu sur une seule page lorsque le projet est enregistré au format graphique. La taille de la page sera modifiée afin que le projet rendu tienne sur une page.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant si un projet doit être rendu sur une seule page lorsque le projet est enregistré au format graphique. |

### setRollUpGanttBars(boolean value) {#setRollUpGanttBars-boolean-}
```
public final void setRollUpGanttBars(boolean value)
```


Définit une valeur indiquant si les sous‑tâches sur la barre de tâche récapitulative doivent être marquées. Pour les sous‑tâches, le champ Rollup indique si les informations sur les barres Gantt des sous‑tâches seront agrégées vers la barre de tâche récapitulative. Pour les tâches récapitulatives, le champ Rollup indique si la barre de tâche récapitulative affiche les barres agrégées. Vous devez définir le champ Rollup des tâches récapitulatives sur Oui pour que les sous‑tâches puissent être agrégées.

--------------------

S'applique uniquement lorsque la vue du diagramme de Gantt est rendue.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant si les sous‑tâches sur la barre de tâche récapitulative doivent être marquées. |

### setStartDate(Date value) {#setStartDate-java.util.Date-}
```
public final void setStartDate(Date value)
```


Définit la date à partir de laquelle le rendu commence.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.Date | la date à partir de laquelle commencer le rendu. |

### setTaskLinkDrawingCallback(TaskLinkDrawingCallbackDelegate value) {#setTaskLinkDrawingCallback-com.aspose.tasks.TaskLinkDrawingCallbackDelegate-}
```
public final void setTaskLinkDrawingCallback(TaskLinkDrawingCallbackDelegate value)
```


Définit un rappel qui peut être utilisé pour personnaliser certains aspects du rendu des liens de tâches.

S'applique uniquement lorsque la vue du diagramme de Gantt est rendue.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [TaskLinkDrawingCallbackDelegate](../../com.aspose.tasks/tasklinkdrawingcallbackdelegate) | un rappel qui peut être utilisé pour personnaliser certains aspects du rendu des liens de tâches. |

### setTextStyles(List&lt;TextStyle&gt; value) {#setTextStyles-java.util.List-com.aspose.tasks.TextStyle--}
```
public final void setTextStyles(List<TextStyle> value)
```


Définit la liste des styles de texte appliqués lors du rendu d'une vue de projet.

--------------------

Ces styles remplacent les styles définis avec GanttCharView.setTextStyles.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.List&lt;com.aspose.tasks.TextStyle&gt; | la liste des styles de texte appliqués lors du rendu d'une vue de projet. |

### setTimescale(int value) {#setTimescale-int-}
```
public final void setTimescale(int value)
```


Définit la valeur `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) qui est utilisée pour contrôler la façon dont l'échelle de temps (si présente) est rendue lorsque le projet est enregistré au format graphique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | int | la valeur du `Timescale`([getTimescale()](../../com.aspose.tasks/saveoptions\#getTimescale--)/[setTimescale(int)](../../com.aspose.tasks/saveoptions\#setTimescale-int-)) qui est utilisée pour contrôler la façon dont l'échelle de temps (si présente) est rendue lorsque le projet est enregistré au format graphique. |

### setTimescaleFitBehavior(int value) {#setTimescaleFitBehavior-int-}
```
public final void setTimescaleFitBehavior(int value)
```


Définit un comportement qui définit comment aligner l'extrémité droite de l'échelle de temps avec la fin de la page.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | un comportement qui définit comment aligner l'extrémité droite de l'échelle de temps avec la fin de la page. |

### setUseGradientBrush(boolean value) {#setUseGradientBrush-boolean-}
```
public void setUseGradientBrush(boolean value)
```


Définit une valeur indiquant si un pinceau dégradé doit être utilisé lors du rendu du diagramme de Gantt.

--------------------

S'applique uniquement lorsque la vue du diagramme de Gantt est rendue.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant si un pinceau dégradé doit être utilisé lors du rendu du diagramme de Gantt. |

### setView(ProjectView value) {#setView-com.aspose.tasks.ProjectView-}
```
public final void setView(ProjectView value)
```


Définit une liste des colonnes de vue à rendre ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). Si non définie, seuls les identifiants de tâche, les noms de tâche, le début et la fin sont rendus. Si les propriétés View et `ViewSettings`([getViewSettings()](../../com.aspose.tasks/saveoptions\#getViewSettings--)/[setViewSettings(View)](../../com.aspose.tasks/saveoptions\#setViewSettings-View-)) sont toutes deux définies, les colonnes de View remplacent celles de ViewSettings.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [ProjectView](../../com.aspose.tasks/projectview) | une liste des colonnes de vue à rendre ([GanttChartColumn](../../com.aspose.tasks/ganttchartcolumn)). |

### setViewSettings(View value) {#setViewSettings-com.aspose.tasks.View-}
```
public final void setViewSettings(View value)
```


Définit une vue (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) à rendre. Vous pouvez utiliser cette option pour spécifier explicitement quelle vue doit être enregistrée aux formats PDF, HTML ou Image. Si cette propriété est définie, la propriété [PresentationFormat](../../com.aspose.tasks/presentationformat) est ignorée lors de l'enregistrement du projet. La vue doit provenir de l'un des écrans suivants ((`Aspose.Tasks.View.Screen`([View.getScreen()](../../com.aspose.tasks/view\#getScreen--)/[View.setScreen(int)](../../com.aspose.tasks/view\#setScreen-int-)))) : (Gantt, TaskSheet, TaskUsage, ResourceSheet, ResourceUsage)

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [View](../../com.aspose.tasks/view) | une vue (`View`([getView()](../../com.aspose.tasks/saveoptions\#getView--)/[setView(ProjectView)](../../com.aspose.tasks/saveoptions\#setView-ProjectView-))) à rendre. |

