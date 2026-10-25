---
title: "TextStyle"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Modifie le style visuel du texte d'un élément dans la vue du projet."
type: docs
weight: 315
url: /fr/java/com.aspose.tasks/textstyle/
---

**Inheritance:**
java.lang.Object
```
public class TextStyle
```

Modifie le style visuel du texte d'un élément dans la vue du projet.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [TextStyle()](#TextStyle--) | Initialise une nouvelle instance de la classe [TextStyle](../../com.aspose.tasks/textstyle) avec les paramètres par défaut. |
| [TextStyle(float fontSize, int fontStyle)](#TextStyle-float-int-) | Initialise une nouvelle instance de la classe [TextStyle](../../com.aspose.tasks/textstyle) avec la police par défaut et la taille et le style de police spécifiés. |
| [TextStyle(int fontStyle)](#TextStyle-int-) | Initialise une nouvelle instance de la classe [TextStyle](../../com.aspose.tasks/textstyle) avec la police par défaut et le style de police spécifié. |
| [TextStyle(FontDescriptor font)](#TextStyle-com.aspose.tasks.FontDescriptor-) | Initialise une nouvelle instance de la classe [TextStyle](../../com.aspose.tasks/textstyle) avec les paramètres de police spécifiés. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getBackgroundColor()](#getBackgroundColor--) | Obtient la couleur d'arrière-plan du style de texte. |
| [getBackgroundPattern()](#getBackgroundPattern--) | Obtient le motif d'arrière-plan du style de texte. |
| [getColor()](#getColor--) | Obtient la couleur du texte. |
| [getFont()](#getFont--) | Obtient la police du style de texte. |
| [getItemType()](#getItemType--) | Obtient le [TextItemType](../../com.aspose.tasks/textitemtype) du style de texte. |
| [setBackgroundColor(Color value)](#setBackgroundColor-java.awt.Color-) | Définit la couleur d'arrière-plan du style de texte. |
| [setBackgroundPattern(int value)](#setBackgroundPattern-int-) | Définit le motif d'arrière-plan du style de texte. |
| [setColor(Color value)](#setColor-java.awt.Color-) | Définit la couleur du texte. |
| [setFont(FontDescriptor value)](#setFont-com.aspose.tasks.FontDescriptor-) | Définit la police du style de texte. |
| [setItemType(int value)](#setItemType-int-) | Définit le [TextItemType](../../com.aspose.tasks/textitemtype) du style de texte. |
### TextStyle() {#TextStyle--}
```
public TextStyle()
```


Initialise une nouvelle instance de la classe [TextStyle](../../com.aspose.tasks/textstyle) avec les paramètres par défaut.

### TextStyle(float fontSize, int fontStyle) {#TextStyle-float-int-}
```
public TextStyle(float fontSize, int fontStyle)
```


Initialise une nouvelle instance de la classe [TextStyle](../../com.aspose.tasks/textstyle) avec la police par défaut et la taille et le style de police spécifiés.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fontSize | float | Taille de la police du TextStyle. |
| fontStyle | int | Style de la police du TextStyle. |

### TextStyle(int fontStyle) {#TextStyle-int-}
```
public TextStyle(int fontStyle)
```


Initialise une nouvelle instance de la classe [TextStyle](../../com.aspose.tasks/textstyle) avec la police par défaut et le style de police spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| fontStyle | int | Style de police à appliquer à la police par défaut. |

### TextStyle(FontDescriptor font) {#TextStyle-com.aspose.tasks.FontDescriptor-}
```
public TextStyle(FontDescriptor font)
```


Initialise une nouvelle instance de la classe [TextStyle](../../com.aspose.tasks/textstyle) avec les paramètres de police spécifiés.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| font | [FontDescriptor](../../com.aspose.tasks/fontdescriptor) | Police du TextStyle. |

### getBackgroundColor() {#getBackgroundColor--}
```
public final Color getBackgroundColor()
```


Obtient la couleur d'arrière-plan du style de texte. `Color`([getBackgroundColor()](../../com.aspose.tasks/textstyle\#getBackgroundColor--)/[setBackgroundColor(java.awt.Color)](../../com.aspose.tasks/textstyle\#setBackgroundColor-java.awt.Color-)).

**Returns:**
java.awt.Color - couleur d'arrière-plan du style de texte.
### getBackgroundPattern() {#getBackgroundPattern--}
```
public final int getBackgroundPattern()
```


Obtient le motif d'arrière-plan du style de texte. `BackgroundPattern`([getBackgroundPattern()](../../com.aspose.tasks/textstyle\#getBackgroundPattern--)/[setBackgroundPattern(int)](../../com.aspose.tasks/textstyle\#setBackgroundPattern-int-)).

**Returns:**
int - motif d'arrière-plan du style de texte.
### getColor() {#getColor--}
```
public final Color getColor()
```


Obtient la couleur du texte.

**Returns:**
java.awt.Color - couleur du texte.
### getFont() {#getFont--}
```
public final FontDescriptor getFont()
```


Obtient la police du style de texte.

**Returns:**
[FontDescriptor](../../com.aspose.tasks/fontdescriptor) - font of the text style.
### getItemType() {#getItemType--}
```
public int getItemType()
```


Obtient le [TextItemType](../../com.aspose.tasks/textitemtype) du style de texte.

**Returns:**
int - [TextItemType](../../com.aspose.tasks/textitemtype) du style de texte.
### setBackgroundColor(Color value) {#setBackgroundColor-java.awt.Color-}
```
public final void setBackgroundColor(Color value)
```


Définit la couleur d'arrière-plan du style de texte. `Color`([getBackgroundColor()](../../com.aspose.tasks/textstyle\#getBackgroundColor--)/[setBackgroundColor(java.awt.Color)](../../com.aspose.tasks/textstyle\#setBackgroundColor-java.awt.Color-)).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.awt.Color | couleur d'arrière-plan du style de texte. |

### setBackgroundPattern(int value) {#setBackgroundPattern-int-}
```
public final void setBackgroundPattern(int value)
```


Définit le motif d'arrière-plan du style de texte. `BackgroundPattern`([getBackgroundPattern()](../../com.aspose.tasks/textstyle\#getBackgroundPattern--)/[setBackgroundPattern(int)](../../com.aspose.tasks/textstyle\#setBackgroundPattern-int-)).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | motif d'arrière-plan du style de texte. |

### setColor(Color value) {#setColor-java.awt.Color-}
```
public final void setColor(Color value)
```


Définit la couleur du texte.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.awt.Color | couleur du texte. |

### setFont(FontDescriptor value) {#setFont-com.aspose.tasks.FontDescriptor-}
```
public final void setFont(FontDescriptor value)
```


Définit la police du style de texte.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [FontDescriptor](../../com.aspose.tasks/fontdescriptor) | police du style de texte. |

### setItemType(int value) {#setItemType-int-}
```
public void setItemType(int value)
```


Définit le [TextItemType](../../com.aspose.tasks/textitemtype) du style de texte.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | int | [TextItemType](../../com.aspose.tasks/textitemtype) du style de texte. |

