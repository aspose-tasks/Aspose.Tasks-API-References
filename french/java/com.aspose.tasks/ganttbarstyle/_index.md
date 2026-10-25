---
title: "GanttBarStyle"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente un style de barre utilisé par MSP dans la vue du diagramme de Gantt."
type: docs
weight: 109
url: /fr/java/com.aspose.tasks/ganttbarstyle/
---

**Inheritance:**
java.lang.Object
```
public class GanttBarStyle
```

Représente un style de barre utilisé par MSP dans la vue du diagramme de Gantt.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [GanttBarStyle()](#GanttBarStyle--) | Initialise une nouvelle instance de la classe [GanttBarStyle](../../com.aspose.tasks/ganttbarstyle). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getBottomBarTextConverter()](#getBottomBarTextConverter--) | Obtient le convertisseur défini par l'utilisateur pour récupérer le texte à afficher en bas de la barre de la tâche. |
| [getBottomField()](#getBottomField--) | Obtient les données à afficher en bas de la barre. |
| [getEndShape()](#getEndShape--) | Obtient une forme de fin de la barre. |
| [getEndShapeColor()](#getEndShapeColor--) | Obtient la couleur de la forme de fin. |
| [getEndShapeType()](#getEndShapeType--) | Obtient le type de la forme de fin. |
| [getFrom()](#getFrom--) | Obtient la position du point de départ de la barre Gantt. |
| [getInsideBarTextConverter()](#getInsideBarTextConverter--) | Obtient le convertisseur défini par l'utilisateur pour récupérer le texte à afficher à l'intérieur de la barre de la tâche. |
| [getInsideField()](#getInsideField--) | Obtient les données à afficher à l'intérieur de la barre. |
| [getLeftBarTextConverter()](#getLeftBarTextConverter--) | Obtient le convertisseur défini par l'utilisateur pour récupérer le texte à afficher à gauche de la barre de la tâche. |
| [getLeftField()](#getLeftField--) | Obtient les données à afficher à gauche de la barre. |
| [getMiddleFillPattern()](#getMiddleFillPattern--) | Obtient le motif de remplissage de la barre Gantt. |
| [getMiddleShape()](#getMiddleShape--) | Obtient une forme centrale de la barre. |
| [getMiddleShapeColor()](#getMiddleShapeColor--) | Obtient une couleur de la forme du milieu. |
| [getName()](#getName--) | Obtient un nom du style. |
| [getParentStyle()](#getParentStyle--) | Obtient le style parent (ou commun) pour le style personnalisé spécifique à la tâche. |
| [getRightBarTextConverter()](#getRightBarTextConverter--) | Obtient le convertisseur défini par l'utilisateur pour obtenir le texte à afficher à droite de la barre de la tâche. |
| [getRightField()](#getRightField--) | Obtient les données à afficher à droite de la barre. |
| [getRow()](#getRow--) | Obtient un numéro de ligne. |
| [getShowForCategories()](#getShowForCategories--) | Obtient les catégories de tâches pour lesquelles le style est appliqué. |
| [getShowForTaskUid()](#getShowForTaskUid--) | Obtient l'identifiant unique d'une tâche pour laquelle le style est appliqué. |
| [getStartShape()](#getStartShape--) | Obtient une forme de départ de la barre. |
| [getStartShapeColor()](#getStartShapeColor--) | Obtient une couleur de la forme de départ. |
| [getStartShapeType()](#getStartShapeType--) | Obtient un type de la forme de départ. |
| [getTo()](#getTo--) | Obtient la position du point final de la barre Gantt. |
| [getTopBarTextConverter()](#getTopBarTextConverter--) | Obtient le convertisseur défini par l'utilisateur pour obtenir le texte à afficher en haut de la barre de la tâche. |
| [getTopField()](#getTopField--) | Obtient les données à afficher en haut de la barre. |
| [setBottomBarTextConverter(TaskBarTextConverter value)](#setBottomBarTextConverter-com.aspose.tasks.TaskBarTextConverter-) | Définit le convertisseur défini par l'utilisateur pour obtenir le texte à afficher en bas de la barre de la tâche. |
| [setBottomField(int value)](#setBottomField-int-) | Définit les données à afficher en bas de la barre. |
| [setEndShape(int value)](#setEndShape-int-) | Définit une forme de fin de la barre. |
| [setEndShapeColor(Color value)](#setEndShapeColor-java.awt.Color-) | Définit une couleur de la forme de fin. |
| [setEndShapeType(int value)](#setEndShapeType-int-) | Définit un type de la forme de fin. |
| [setFrom(int value)](#setFrom-int-) | Définit la position du point de départ de la barre Gantt. |
| [setInsideBarTextConverter(TaskBarTextConverter value)](#setInsideBarTextConverter-com.aspose.tasks.TaskBarTextConverter-) | Définit le convertisseur défini par l'utilisateur pour obtenir le texte à afficher à l'intérieur de la barre de la tâche. |
| [setInsideField(int value)](#setInsideField-int-) | Définit les données à afficher à l'intérieur de la barre. |
| [setLeftBarTextConverter(TaskBarTextConverter value)](#setLeftBarTextConverter-com.aspose.tasks.TaskBarTextConverter-) | Définit le convertisseur défini par l'utilisateur pour obtenir le texte à afficher à gauche de la barre de la tâche. |
| [setLeftField(int value)](#setLeftField-int-) | Définit les données à afficher à gauche de la barre. |
| [setMiddleFillPattern(int value)](#setMiddleFillPattern-int-) | Définit un motif de remplissage de la barre Gantt. |
| [setMiddleShape(int value)](#setMiddleShape-int-) | Définit une forme intermédiaire de la barre. |
| [setMiddleShapeColor(Color value)](#setMiddleShapeColor-java.awt.Color-) | Définit une couleur de la forme intermédiaire. |
| [setName(String value)](#setName-java.lang.String-) | Définit un nom du style. |
| [setParentStyle(GanttBarStyle value)](#setParentStyle-com.aspose.tasks.GanttBarStyle-) | Définit le style parent (ou commun) pour le style personnalisé spécifique à la tâche. |
| [setRightBarTextConverter(TaskBarTextConverter value)](#setRightBarTextConverter-com.aspose.tasks.TaskBarTextConverter-) | Définit le convertisseur défini par l'utilisateur pour obtenir le texte à afficher à droite de la barre de la tâche. |
| [setRightField(int value)](#setRightField-int-) | Définit les données à afficher à droite de la barre. |
| [setRow(int value)](#setRow-int-) | Définit un numéro de ligne. |
| [setShowForCategories(List&lt;Integer&gt; value)](#setShowForCategories-java.util.List-java.lang.Integer--) | Définit les catégories de tâches auxquelles le style est appliqué. |
| [setShowForTaskUid(Integer value)](#setShowForTaskUid-java.lang.Integer-) | Définit l'Identifiant unique d'une tâche pour laquelle le style est appliqué. |
| [setStartShape(int value)](#setStartShape-int-) | Définit une forme de départ de la barre. |
| [setStartShapeColor(Color value)](#setStartShapeColor-java.awt.Color-) | Définit une couleur de la forme de départ. |
| [setStartShapeType(int value)](#setStartShapeType-int-) | Définit un type de la forme de départ. |
| [setTo(int value)](#setTo-int-) | Définit la position du point de fin de la barre Gantt. |
| [setTopBarTextConverter(TaskBarTextConverter value)](#setTopBarTextConverter-com.aspose.tasks.TaskBarTextConverter-) | Définit le convertisseur défini par l'utilisateur pour obtenir le texte à afficher en haut de la barre de la tâche. |
| [setTopField(int value)](#setTopField-int-) | Définit les données à afficher en haut de la barre. |
### GanttBarStyle() {#GanttBarStyle--}
```
public GanttBarStyle()
```


Initialise une nouvelle instance de la classe [GanttBarStyle](../../com.aspose.tasks/ganttbarstyle).

### getBottomBarTextConverter() {#getBottomBarTextConverter--}
```
public final TaskBarTextConverter getBottomBarTextConverter()
```


Obtient le convertisseur défini par l'utilisateur pour obtenir le texte à afficher en bas de la barre de la tâche. Remplace la valeur de `BottomField`([getBottomField()](../../com.aspose.tasks/ganttbarstyle\#getBottomField--)/[setBottomField(int)](../../com.aspose.tasks/ganttbarstyle\#setBottomField-int-)) propriété.

--------------------

N'est pas conservé dans le format MPP.

**Returns:**
[TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) - user-defined converter to get text to render on the bottom of the task's bar.
### getBottomField() {#getBottomField--}
```
public final int getBottomField()
```


Obtient les données à afficher en bas de la barre. [Field](../../com.aspose.tasks/field).

**Returns:**
int - données à afficher en bas de la barre.
### getEndShape() {#getEndShape--}
```
public final int getEndShape()
```


Obtient une forme de fin de la barre.

**Returns:**
int - une forme de fin de la barre.
### getEndShapeColor() {#getEndShapeColor--}
```
public final Color getEndShapeColor()
```


Obtient la couleur de la forme de fin.

**Returns:**
java.awt.Color - une couleur de la forme de fin.
### getEndShapeType() {#getEndShapeType--}
```
public final int getEndShapeType()
```


Obtient un type de la forme de fin. [GanttBarType](../../com.aspose.tasks/ganttbartype).

**Returns:**
int - un type de la forme de fin.
### getFrom() {#getFrom--}
```
public final int getFrom()
```


Obtient une position du point de départ de la barre Gantt. [Field](../../com.aspose.tasks/field).

**Returns:**
int - une position du point de départ de la barre Gantt.
### getInsideBarTextConverter() {#getInsideBarTextConverter--}
```
public final TaskBarTextConverter getInsideBarTextConverter()
```


Obtient le convertisseur défini par l'utilisateur pour obtenir le texte à rendre à l'intérieur de la barre de la tâche. Remplace la valeur de `InsideField`([getInsideField()](../../com.aspose.tasks/ganttbarstyle\#getInsideField--)/[setInsideField(int)](../../com.aspose.tasks/ganttbarstyle\#setInsideField-int-)) propriété.

--------------------

N'est pas conservé dans le format MPP.

**Returns:**
[TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) - user-defined converter to get text to render inside of the task's bar.
### getInsideField() {#getInsideField--}
```
public final int getInsideField()
```


Obtient les données à afficher à l'intérieur de la barre. [Field](../../com.aspose.tasks/field).

**Returns:**
int - données à afficher à l'intérieur de la barre.
### getLeftBarTextConverter() {#getLeftBarTextConverter--}
```
public final TaskBarTextConverter getLeftBarTextConverter()
```


Obtient le convertisseur défini par l'utilisateur pour obtenir le texte à rendre à gauche de la barre de la tâche. Remplace la valeur de `LeftField`([getLeftField()](../../com.aspose.tasks/ganttbarstyle\#getLeftField--)/[setLeftField(int)](../../com.aspose.tasks/ganttbarstyle\#setLeftField-int-)) propriété.

--------------------

N'est pas conservé dans le format MPP.

**Returns:**
[TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) - user-defined converter to get text to render on the left of the task's bar.
### getLeftField() {#getLeftField--}
```
public final int getLeftField()
```


Obtient les données à afficher à gauche de la barre. [Field](../../com.aspose.tasks/field).

**Returns:**
int - données à afficher à gauche de la barre.
### getMiddleFillPattern() {#getMiddleFillPattern--}
```
public final int getMiddleFillPattern()
```


Obtient le motif de remplissage de la barre Gantt.

**Returns:**
int - un motif de remplissage de la barre Gantt.
### getMiddleShape() {#getMiddleShape--}
```
public final int getMiddleShape()
```


Obtient une forme centrale de la barre.

**Returns:**
int - une forme centrale de la barre.
### getMiddleShapeColor() {#getMiddleShapeColor--}
```
public final Color getMiddleShapeColor()
```


Obtient une couleur de la forme du milieu.

**Returns:**
java.awt.Color - une couleur de la forme centrale.
### getName() {#getName--}
```
public final String getName()
```


Obtient un nom du style.

**Returns:**
java.lang.String - un nom du style.
### getParentStyle() {#getParentStyle--}
```
public final GanttBarStyle getParentStyle()
```


Obtient le style parent (ou commun) pour le style personnalisé spécifique à la tâche.

--------------------

Une tâche peut avoir plusieurs styles personnalisés avec différents styles parents. Par exemple, considérez une tâche ayant un style personnalisé avec le style parent "Critical" et un autre style avec le style parent "Normal". En résumé, si la tâche est critique, le premier style est appliqué. Si la tâche devient non critique, le second style est appliqué (cette logique est héritée de Microsoft Project Professional).

**Returns:**
[GanttBarStyle](../../com.aspose.tasks/ganttbarstyle) - parent (or common) style for custom task-specific style.
### getRightBarTextConverter() {#getRightBarTextConverter--}
```
public final TaskBarTextConverter getRightBarTextConverter()
```


Obtient le convertisseur défini par l'utilisateur pour obtenir le texte à rendre à droite de la barre de la tâche. Remplace la valeur de `RightField`([getRightField()](../../com.aspose.tasks/ganttbarstyle\#getRightField--)/[setRightField(int)](../../com.aspose.tasks/ganttbarstyle\#setRightField-int-)) propriété.

--------------------

N'est pas conservé dans le format MPP.

**Returns:**
[TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) - user-defined converter to get text to render on the right of the task's bar.
### getRightField() {#getRightField--}
```
public final int getRightField()
```


Obtient les données à afficher à droite de la barre. [Field](../../com.aspose.tasks/field).

**Returns:**
int - données à afficher à droite de la barre.
### getRow() {#getRow--}
```
public final int getRow()
```


Obtient un numéro de ligne.

--------------------

Peut être de 1 à 4 (1 est la valeur par défaut).

**Returns:**
int - un numéro de ligne.
### getShowForCategories() {#getShowForCategories--}
```
public final List<Integer> getShowForCategories()
```


Obtient les catégories de tâches pour lesquelles le style est appliqué. S'applique aux styles parents (ou communs) des barres dans le diagramme de Gantt (voir `GanttChartView.BarStyles`([GanttChartView.getBarStyles()](../../com.aspose.tasks/ganttchartview\#getBarStyles--))).

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - catégories de tâches pour lesquelles le style est appliqué.
### getShowForTaskUid() {#getShowForTaskUid--}
```
public final Integer getShowForTaskUid()
```


Obtient l'identifiant unique d'une tâche pour laquelle le style est appliqué. S'applique aux styles spécifiques aux tâches des barres dans le diagramme de Gantt (voir `GanttChartView.CustomBarStyles`([GanttChartView.getCustomBarStyles()](../../com.aspose.tasks/ganttchartview\#getCustomBarStyles--))).

**Returns:**
java.lang.Integer - Identifiant unique d'une tâche pour laquelle le style est appliqué.
### getStartShape() {#getStartShape--}
```
public final int getStartShape()
```


Obtient une forme de départ de la barre.

**Returns:**
int - une forme de départ de la barre.
### getStartShapeColor() {#getStartShapeColor--}
```
public final Color getStartShapeColor()
```


Obtient une couleur de la forme de départ.

**Returns:**
java.awt.Color - une couleur de la forme de départ.
### getStartShapeType() {#getStartShapeType--}
```
public final int getStartShapeType()
```


Obtient un type de la forme de départ.

**Returns:**
int - un type de la forme de départ.
### getTo() {#getTo--}
```
public final int getTo()
```


Obtient la position du point final de la barre Gantt.

**Returns:**
int - une position du point d'arrivée de la barre Gantt.
### getTopBarTextConverter() {#getTopBarTextConverter--}
```
public final TaskBarTextConverter getTopBarTextConverter()
```


Obtient le convertisseur défini par l'utilisateur pour obtenir le texte à rendre en haut de la barre de la tâche. Remplace la valeur de `TopField`([getTopField()](../../com.aspose.tasks/ganttbarstyle\#getTopField--)/[setTopField(int)](../../com.aspose.tasks/ganttbarstyle\#setTopField-int-)) propriété.

--------------------

N'est pas conservé dans le format MPP.

**Returns:**
[TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) - user-defined converter to get text to render on the top of the task's bar.
### getTopField() {#getTopField--}
```
public final int getTopField()
```


Obtient les données à afficher en haut de la barre.

**Returns:**
int - données à afficher en haut de la barre.
### setBottomBarTextConverter(TaskBarTextConverter value) {#setBottomBarTextConverter-com.aspose.tasks.TaskBarTextConverter-}
```
public final void setBottomBarTextConverter(TaskBarTextConverter value)
```


Définit le convertisseur défini par l'utilisateur pour obtenir le texte à rendre en bas de la barre de la tâche. Remplace la valeur de `BottomField`([getBottomField()](../../com.aspose.tasks/ganttbarstyle\#getBottomField--)/[setBottomField(int)](../../com.aspose.tasks/ganttbarstyle\#setBottomField-int-)) propriété.

--------------------

N'est pas conservé dans le format MPP.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) | convertisseur défini par l'utilisateur pour obtenir le texte à rendre en bas de la barre de la tâche. |

### setBottomField(int value) {#setBottomField-int-}
```
public final void setBottomField(int value)
```


Définit les données à afficher en bas de la barre. [Field](../../com.aspose.tasks/field).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | données à afficher en bas de la barre. |

### setEndShape(int value) {#setEndShape-int-}
```
public final void setEndShape(int value)
```


Définit une forme de fin de la barre.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | une forme de fin de la barre. |

### setEndShapeColor(Color value) {#setEndShapeColor-java.awt.Color-}
```
public final void setEndShapeColor(Color value)
```


Définit une couleur de la forme de fin.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.awt.Color | une couleur de la forme de fin. |

### setEndShapeType(int value) {#setEndShapeType-int-}
```
public final void setEndShapeType(int value)
```


Définit un type de forme de fin. [GanttBarType](../../com.aspose.tasks/ganttbartype).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | un type de forme de fin. |

### setFrom(int value) {#setFrom-int-}
```
public final void setFrom(int value)
```


Définit la position du point de départ de la barre Gantt. [Field](../../com.aspose.tasks/field).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | une position du point de départ de la barre Gantt. |

### setInsideBarTextConverter(TaskBarTextConverter value) {#setInsideBarTextConverter-com.aspose.tasks.TaskBarTextConverter-}
```
public final void setInsideBarTextConverter(TaskBarTextConverter value)
```


Définit le convertisseur défini par l'utilisateur pour obtenir le texte à rendre à l'intérieur de la barre de la tâche. Remplace la valeur de `InsideField`([getInsideField()](../../com.aspose.tasks/ganttbarstyle\#getInsideField--)/[setInsideField(int)](../../com.aspose.tasks/ganttbarstyle\#setInsideField-int-)) propriété.

--------------------

N'est pas conservé dans le format MPP.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) | convertisseur défini par l'utilisateur pour obtenir le texte à rendre à l'intérieur de la barre de la tâche. |

### setInsideField(int value) {#setInsideField-int-}
```
public final void setInsideField(int value)
```


Définit les données à afficher à l'intérieur de la barre. [Field](../../com.aspose.tasks/field).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | données à afficher à l'intérieur de la barre. |

### setLeftBarTextConverter(TaskBarTextConverter value) {#setLeftBarTextConverter-com.aspose.tasks.TaskBarTextConverter-}
```
public final void setLeftBarTextConverter(TaskBarTextConverter value)
```


Définit le convertisseur défini par l'utilisateur pour obtenir le texte à rendre à gauche de la barre de la tâche. Remplace la valeur de `LeftField`([getLeftField()](../../com.aspose.tasks/ganttbarstyle\#getLeftField--)/[setLeftField(int)](../../com.aspose.tasks/ganttbarstyle\#setLeftField-int-)) propriété.

--------------------

N'est pas conservé dans le format MPP.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) | convertisseur défini par l'utilisateur pour obtenir le texte à rendre à gauche de la barre de la tâche. |

### setLeftField(int value) {#setLeftField-int-}
```
public final void setLeftField(int value)
```


Définit les données à afficher à gauche de la barre. [Field](../../com.aspose.tasks/field).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | données à afficher à gauche de la barre. |

### setMiddleFillPattern(int value) {#setMiddleFillPattern-int-}
```
public final void setMiddleFillPattern(int value)
```


Définit un motif de remplissage de la barre Gantt.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | un motif de remplissage de la barre Gantt. |

### setMiddleShape(int value) {#setMiddleShape-int-}
```
public final void setMiddleShape(int value)
```


Définit une forme intermédiaire de la barre.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | une forme du milieu de la barre. |

### setMiddleShapeColor(Color value) {#setMiddleShapeColor-java.awt.Color-}
```
public final void setMiddleShapeColor(Color value)
```


Définit une couleur de la forme intermédiaire.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.awt.Color | une couleur de la forme du milieu. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Définit un nom du style.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | un nom du style. |

### setParentStyle(GanttBarStyle value) {#setParentStyle-com.aspose.tasks.GanttBarStyle-}
```
public final void setParentStyle(GanttBarStyle value)
```


Définit le style parent (ou commun) pour le style personnalisé spécifique à la tâche.

--------------------

Une tâche peut avoir plusieurs styles personnalisés avec différents styles parents. Par exemple, considérez une tâche ayant un style personnalisé avec le style parent "Critical" et un autre style avec le style parent "Normal". En résumé, si la tâche est critique, le premier style est appliqué. Si la tâche devient non critique, le second style est appliqué (cette logique est héritée de Microsoft Project Professional).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [GanttBarStyle](../../com.aspose.tasks/ganttbarstyle) | style parent (ou commun) pour un style personnalisé spécifique à la tâche. |

### setRightBarTextConverter(TaskBarTextConverter value) {#setRightBarTextConverter-com.aspose.tasks.TaskBarTextConverter-}
```
public final void setRightBarTextConverter(TaskBarTextConverter value)
```


Définit le convertisseur défini par l'utilisateur pour obtenir le texte à rendre à droite de la barre de la tâche. Remplace la valeur de `RightField`([getRightField()](../../com.aspose.tasks/ganttbarstyle\#getRightField--)/[setRightField(int)](../../com.aspose.tasks/ganttbarstyle\#setRightField-int-)) propriété.

--------------------

N'est pas conservé dans le format MPP.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) | convertisseur défini par l'utilisateur pour obtenir le texte à afficher à droite de la barre de la tâche. |

### setRightField(int value) {#setRightField-int-}
```
public final void setRightField(int value)
```


Définit les données à afficher à droite de la barre. [Field](../../com.aspose/tasks/field).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | données à afficher à droite de la barre. |

### setRow(int value) {#setRow-int-}
```
public final void setRow(int value)
```


Définit un numéro de ligne.

--------------------

Peut être de 1 à 4 (1 est la valeur par défaut).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | un numéro de ligne. |

### setShowForCategories(List&lt;Integer&gt; value) {#setShowForCategories-java.util.List-java.lang.Integer--}
```
public final void setShowForCategories(List<Integer> value)
```


Définit les catégories de tâches pour lesquelles le style est appliqué. S'applique aux styles parent (ou communs) des barres dans le diagramme de Gantt (voir `GanttChartView.BarStyles`([GanttChartView.getBarStyles()](../../com.aspose.tasks/ganttchartview\#getBarStyles--))).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.List&lt;java.lang.Integer&gt; | catégories de tâches pour lesquelles le style est appliqué. |

### setShowForTaskUid(Integer value) {#setShowForTaskUid-java.lang.Integer-}
```
public final void setShowForTaskUid(Integer value)
```


Définit l'Identifiant unique d'une tâche pour laquelle le style est appliqué. S'applique aux styles spécifiques aux tâches des barres dans le diagramme de Gantt (voir `GanttChartView.CustomBarStyles`([GanttChartView.getCustomBarStyles()](../../com.aspose.tasks/ganttchartview\#getCustomBarStyles--))).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.Integer | Identifiant unique d'une tâche pour laquelle le style est appliqué. |

### setStartShape(int value) {#setStartShape-int-}
```
public final void setStartShape(int value)
```


Définit une forme de départ de la barre.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | une forme de départ de la barre. |

### setStartShapeColor(Color value) {#setStartShapeColor-java.awt.Color-}
```
public final void setStartShapeColor(Color value)
```


Définit une couleur de la forme de départ.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.awt.Color | une couleur de la forme de départ. |

### setStartShapeType(int value) {#setStartShapeType-int-}
```
public final void setStartShapeType(int value)
```


Définit un type de la forme de départ.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | un type de forme de départ. |

### setTo(int value) {#setTo-int-}
```
public final void setTo(int value)
```


Définit la position du point de fin de la barre Gantt.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | une position du point de fin de la barre de Gantt. |

### setTopBarTextConverter(TaskBarTextConverter value) {#setTopBarTextConverter-com.aspose.tasks.TaskBarTextConverter-}
```
public final void setTopBarTextConverter(TaskBarTextConverter value)
```


Définit le convertisseur défini par l'utilisateur pour obtenir le texte à afficher en haut de la barre de la tâche. Remplace la valeur de la propriété `TopField`([getTopField()](../../com.aspose.tasks/ganttbarstyle\#getTopField--)/[setTopField(int)](../../com.aspose.tasks/ganttbarstyle\#setTopField-int-)).

--------------------

N'est pas conservé dans le format MPP.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [TaskBarTextConverter](../../com.aspose.tasks/taskbartextconverter) | convertisseur défini par l'utilisateur pour obtenir le texte à afficher en haut de la barre de la tâche. |

### setTopField(int value) {#setTopField-int-}
```
public final void setTopField(int value)
```


Définit les données à afficher en haut de la barre.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | données à afficher en haut de la barre. |

