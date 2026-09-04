---
title: "TableTextStyle"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente un style de texte dans une table de vue."
type: docs
weight: 288
url: /fr/java/com.aspose.tasks/tabletextstyle/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.TextStyle](../../com.aspose.tasks/textstyle)
```
public class TableTextStyle extends TextStyle
```

Représente un style de texte dans une table de vue.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [TableTextStyle(int rowUid)](#TableTextStyle-int-) | Initialise une nouvelle instance de la classe [TableTextStyle](../../com.aspose.tasks/tabletextstyle). |
| [TableTextStyle(int rowUid, FontDescriptor font)](#TableTextStyle-int-com.aspose.tasks.FontDescriptor-) | Initialise une nouvelle instance de la classe [TableTextStyle](../../com.aspose.tasks/tabletextstyle) avec la police spécifiée. |
| [TableTextStyle(int rowUid, float fontSize, int fontStyle)](#TableTextStyle-int-float-int-) | Initialise une nouvelle instance de la classe [TableTextStyle](../../com.aspose.tasks/tabletextstyle) avec la taille de police et le style de police spécifiés. |
| [TableTextStyle(int rowUid, int fontStyle)](#TableTextStyle-int-int-) | Initialise une nouvelle instance de la classe [TableTextStyle](../../com.aspose.tasks/tabletextstyle) avec les paramètres de police par défaut et le style de police spécifié. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getField()](#getField--) | Obtient le champ auquel le style doit être appliqué. |
| [getItemType()](#getItemType--) | Renvoie le type d'élément texte. |
| [getRowUid()](#getRowUid--) | Obtient l'identifiant unique d'une ligne. |
| [setField(int value)](#setField-int-) | Définit le champ auquel le style doit être appliqué. |
### TableTextStyle(int rowUid) {#TableTextStyle-int-}
```
public TableTextStyle(int rowUid)
```


Initialise une nouvelle instance de la classe [TableTextStyle](../../com.aspose.tasks/tabletextstyle).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rowUid | int | Un identifiant unique de ligne spécifié. |

### TableTextStyle(int rowUid, FontDescriptor font) {#TableTextStyle-int-com.aspose.tasks.FontDescriptor-}
```
public TableTextStyle(int rowUid, FontDescriptor font)
```


Initialise une nouvelle instance de la classe [TableTextStyle](../../com.aspose.tasks/tabletextstyle) avec la police spécifiée.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rowUid | int | Un identifiant unique de ligne spécifié. |
| font | [FontDescriptor](../../com.aspose.tasks/fontdescriptor) | Une police sur laquelle un style de texte est basé. |

### TableTextStyle(int rowUid, float fontSize, int fontStyle) {#TableTextStyle-int-float-int-}
```
public TableTextStyle(int rowUid, float fontSize, int fontStyle)
```


Initialise une nouvelle instance de la classe [TableTextStyle](../../com.aspose.tasks/tabletextstyle) avec la taille de police et le style de police spécifiés.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rowUid | int | Un identifiant unique de ligne spécifié. |
| fontSize | float | Taille d'une police sur laquelle un style de texte est basé. |
| fontStyle | int | Style de police. |

### TableTextStyle(int rowUid, int fontStyle) {#TableTextStyle-int-int-}
```
public TableTextStyle(int rowUid, int fontStyle)
```


Initialise une nouvelle instance de la classe [TableTextStyle](../../com.aspose.tasks/tabletextstyle) avec les paramètres de police par défaut et le style de police spécifié.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| rowUid | int | Un identifiant unique de ligne spécifié. |
| fontStyle | int | Style de police. |

### getField() {#getField--}
```
public final int getField()
```


Obtient un champ auquel le style doit être appliqué. `Field`([getField()](../../com.aspose.tasks/tabletextstyle\#getField--)/[setField(int)](../../com.aspose.tasks/tabletextstyle\#setField-int-)).

**Returns:**
int - un champ auquel le style doit être appliqué.
### getItemType() {#getItemType--}
```
public int getItemType()
```


Renvoie le type d'élément texte.

**Returns:**
int - valeur du type énuméré TextItemType.
### getRowUid() {#getRowUid--}
```
public final int getRowUid()
```


Obtient l'identifiant unique d'une ligne.

--------------------

Retourne -1 si le style doit être appliqué à toutes les lignes d'une vue.

**Returns:**
int - un identifiant unique de ligne.
### setField(int value) {#setField-int-}
```
public final void setField(int value)
```


Définit un champ auquel le style doit être appliqué. `Field`([getField()](../../com.aspose.tasks/tabletextstyle\#getField--)/[setField(int)](../../com.aspose.tasks/tabletextstyle\#setField-int-)).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | un champ auquel le style doit être appliqué. |

