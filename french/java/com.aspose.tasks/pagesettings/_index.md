---
title: "PageSettings"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente les paramètres d'impression pour une page de la vue du projet."
type: docs
weight: 181
url: /fr/java/com.aspose.tasks/pagesettings/
---

**Inheritance:**
java.lang.Object
```
public class PageSettings
```

Représente les paramètres d'impression pour une page de la vue du projet.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [PageSettings()](#PageSettings--) | Initialise une nouvelle instance de la classe [PageSettings](../../com.aspose.tasks/pagesettings). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getAdjustToPercentOfNormalSize()](#getAdjustToPercentOfNormalSize--) | Obtient une valeur indiquant s'il faut ajuster l'impression au pourcentage spécifié (`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) de la taille normale. |
| [getFirstPageNumber()](#getFirstPageNumber--) | Obtient le numéro de première page pour l'impression. |
| [getPagesInHeight()](#getPagesInHeight--) | Obtient le nombre de pages en hauteur à imprimer. |
| [getPagesInWidth()](#getPagesInWidth--) | Obtient le nombre de pages en largeur à imprimer. |
| [getPaperSize()](#getPaperSize--) | Obtient une taille de papier. |
| [getPaperSizeId()](#getPaperSizeId--) | Obtient un entier représentant l'une des valeurs de PrinterPaperSize ou un identifiant de taille de page personnalisé. |
| [getPercentOfNormalSize()](#getPercentOfNormalSize--) | Obtient un pourcentage de la taille normale auquel ajuster l'impression. |
| [isPortrait()](#isPortrait--) | Obtient une valeur indiquant si l'orientation de la page est portrait ; renvoie false si l'orientation de la page est paysage. |
| [setAdjustToPercentOfNormalSize(boolean value)](#setAdjustToPercentOfNormalSize-boolean-) | Définit une valeur indiquant s'il faut ajuster l'impression au pourcentage spécifié (`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) de la taille normale. |
| [setFirstPageNumber(short value)](#setFirstPageNumber-short-) | Définit le numéro de première page pour l'impression. |
| [setPagesInHeight(int value)](#setPagesInHeight-int-) | Définit le nombre de pages en hauteur à imprimer. |
| [setPagesInWidth(int value)](#setPagesInWidth-int-) | Définit le nombre de pages en largeur à imprimer. |
| [setPaperSize(int value)](#setPaperSize-int-) | Définit une taille de papier. |
| [setPaperSizeId(int value)](#setPaperSizeId-int-) | Définit un entier représentant l'une des valeurs de PrinterPaperSize ou un identifiant de taille de page personnalisé. |
| [setPercentOfNormalSize(int value)](#setPercentOfNormalSize-int-) | Définit un pourcentage de la taille normale auquel ajuster l'impression. |
| [setPortrait(boolean value)](#setPortrait-boolean-) | Définit une valeur indiquant si l'orientation de la page est portrait ; renvoie false si l'orientation de la page est paysage. |
### PageSettings() {#PageSettings--}
```
public PageSettings()
```


Initialise une nouvelle instance de la classe [PageSettings](../../com.aspose/tasks/pagesettings). Représente les paramètres d'impression pour une page de la vue du projet.

### getAdjustToPercentOfNormalSize() {#getAdjustToPercentOfNormalSize--}
```
public final boolean getAdjustToPercentOfNormalSize()
```


Obtient une valeur indiquant s'il faut ajuster l'impression au pourcentage spécifié (`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) de la taille normale.

--------------------

N'est pas efficace lorsque le projet est rendu au format HTML.

**Returns:**
booléen - une valeur indiquant s'il faut ajuster l'impression au pourcentage spécifié (`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) de la taille normale.
### getFirstPageNumber() {#getFirstPageNumber--}
```
public final short getFirstPageNumber()
```


Obtient le numéro de première page pour l'impression.

**Returns:**
short - le numéro de première page pour l'impression.
### getPagesInHeight() {#getPagesInHeight--}
```
public final int getPagesInHeight()
```


Obtient le nombre de pages en hauteur à imprimer.

**Returns:**
int - le nombre de pages en hauteur à imprimer.
### getPagesInWidth() {#getPagesInWidth--}
```
public final int getPagesInWidth()
```


Obtient le nombre de pages en largeur à imprimer.

**Returns:**
int - le nombre de pages en largeur à imprimer.
### getPaperSize() {#getPaperSize--}
```
public final int getPaperSize()
```


Obtient une taille de papier. Peut être l'une des valeurs de l'énumération [PrinterPaperSize](../../com.aspose/tasks/printerpapersize).

**Returns:**
int - une taille de papier.
### getPaperSizeId() {#getPaperSizeId--}
```
public final int getPaperSizeId()
```


Obtient un entier représentant l'une des valeurs de PrinterPaperSize ou un identifiant de taille de page personnalisé. Cette valeur peut être utilisée pour obtenir PaperSize à partir des paramètres du système d'exploitation ().

**Returns:**
int - un entier représentant l'une des valeurs de PrinterPaperSize ou un identifiant de taille de page personnalisé.
### getPercentOfNormalSize() {#getPercentOfNormalSize--}
```
public final int getPercentOfNormalSize()
```


Obtient un pourcentage de la taille normale auquel ajuster l'impression.

**Returns:**
int - un pourcentage de la taille normale auquel ajuster l'impression.
### isPortrait() {#isPortrait--}
```
public final boolean isPortrait()
```


Obtient une valeur indiquant si l'orientation de la page est portrait ; renvoie false si l'orientation de la page est paysage.

--------------------

S'applique lors du rendu lorsque SaveOptions.getPageSize() == PageSize.DefinedInView.

**Returns:**
boolean - une valeur indiquant si l'orientation de la page est portrait ; renvoie false si l'orientation de la page est paysage.
### setAdjustToPercentOfNormalSize(boolean value) {#setAdjustToPercentOfNormalSize-boolean-}
```
public final void setAdjustToPercentOfNormalSize(boolean value)
```


Définit une valeur indiquant s'il faut ajuster l'impression au pourcentage spécifié (`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) de la taille normale.

--------------------

N'est pas efficace lorsque le projet est rendu au format HTML.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | boolean | une valeur indiquant s'il faut ajuster l'impression au pourcentage spécifié (`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose.tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose.tasks/pagesettings\#setPercentOfNormalSize-int-))) de la taille normale. |

### setFirstPageNumber(short value) {#setFirstPageNumber-short-}
```
public final void setFirstPageNumber(short value)
```


Définit le numéro de première page pour l'impression.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | short | un numéro de première page pour l'impression. |

### setPagesInHeight(int value) {#setPagesInHeight-int-}
```
public final void setPagesInHeight(int value)
```


Définit le nombre de pages en hauteur à imprimer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | un nombre de pages en hauteur à imprimer. |

### setPagesInWidth(int value) {#setPagesInWidth-int-}
```
public final void setPagesInWidth(int value)
```


Définit le nombre de pages en largeur à imprimer.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | un nombre de pages en largeur à imprimer. |

### setPaperSize(int value) {#setPaperSize-int-}
```
public final void setPaperSize(int value)
```


Définit une taille de papier. Peut être l'une des valeurs de l'énumération [PrinterPaperSize](../../com.aspose.tasks/printerpapersize).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | une taille de papier. |

### setPaperSizeId(int value) {#setPaperSizeId-int-}
```
public final void setPaperSizeId(int value)
```


Définit un entier représentant l'une des valeurs de PrinterPaperSize ou un identifiant de taille de page personnalisé. Cette valeur peut être utilisée pour obtenir PaperSize à partir des paramètres du système d'exploitation ().

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | un entier représentant l'une des valeurs de PrinterPaperSize ou un identifiant de taille de page personnalisé. |

### setPercentOfNormalSize(int value) {#setPercentOfNormalSize-int-}
```
public final void setPercentOfNormalSize(int value)
```


Définit un pourcentage de la taille normale auquel ajuster l'impression.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | un pourcentage de la taille normale auquel ajuster l'impression. |

### setPortrait(boolean value) {#setPortrait-boolean-}
```
public final void setPortrait(boolean value)
```


Définit une valeur indiquant si l'orientation de la page est portrait ; renvoie false si l'orientation de la page est paysage.

--------------------

S'applique lors du rendu lorsque SaveOptions.getPageSize() == PageSize.DefinedInView.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant si l'orientation de la page est portrait ; renvoie false si l'orientation de la page est paysage. |

