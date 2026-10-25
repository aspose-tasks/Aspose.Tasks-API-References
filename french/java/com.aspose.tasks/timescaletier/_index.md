---
title: "TimescaleTier"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente un niveau unique de l'échelle de temps sur un diagramme de Gantt."
type: docs
weight: 325
url: /fr/java/com.aspose.tasks/timescaletier/
---

**Inheritance:**
java.lang.Object
```
public final class TimescaleTier
```

Représente un niveau unique de l'échelle de temps sur un diagramme de Gantt.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [TimescaleTier()](#TimescaleTier--) | Initialise une nouvelle instance de la classe [TimescaleTier](../../com.aspose.tasks/timescaletier). |
| [TimescaleTier(int unit, int count)](#TimescaleTier-int-int-) | Initialise une nouvelle instance de la classe [TimescaleTier](../../com.aspose.tasks/timescaletier). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getAlignment()](#getAlignment--) | Obtient la façon d'aligner les libellés à l'intérieur de chaque période de temps du niveau ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)). |
| [getCount()](#getCount--) | Obtient l'intervalle d'unité de temps dans lequel afficher les libellés pour le niveau. |
| [getDateTimeConverter()](#getDateTimeConverter--) | Obtient une fonction de rappel pour gérer le rendu du repère de date dans ce niveau. |
| [getLabel()](#getLabel--) | Obtient le libellé de date [DateLabel](../../com.aspose.tasks/datelabel) pour le niveau d'échelle de temps. |
| [getRenderLabelOnEachPage()](#getRenderLabelOnEachPage--) | Obtient le drapeau qui définit si les libellés de date doivent être rendus sur chaque page lorsqu'une période de temps s'étend sur plusieurs pages. |
| [getShowTicks()](#getShowTicks--) | Obtient une valeur indiquant s'il faut afficher les marques de repère qui séparent les périodes de temps dans le niveau. |
| [getUnit()](#getUnit--) | Obtient l'unité d'échelle de temps [TimescaleUnit](../../com.aspose.tasks/timescaleunit) pour le niveau d'échelle de temps. |
| [getUsesFiscalYear()](#getUsesFiscalYear--) | Obtient une valeur indiquant s'il faut baser les libellés du niveau sur l'année fiscale. |
| [setAlignment(int value)](#setAlignment-int-) | Définit la façon d'aligner les libellés à l'intérieur de chaque période de temps du niveau ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)). |
| [setCount(int value)](#setCount-int-) | Définit l'intervalle d'unité de temps dans lequel afficher les libellés pour le niveau. |
| [setDateTimeConverter(DateTimeConverter value)](#setDateTimeConverter-com.aspose.tasks.DateTimeConverter-) | Définit une fonction de rappel pour gérer le rendu du repère de date dans ce niveau. |
| [setLabel(int value)](#setLabel-int-) | Définit le libellé de date [DateLabel](../../com.aspose.tasks/datelabel) pour le niveau d'échelle de temps. |
| [setRenderLabelOnEachPage(boolean value)](#setRenderLabelOnEachPage-boolean-) | Définit le drapeau qui indique si les libellés de date doivent être rendus sur chaque page lorsqu'une période de temps s'étend sur plusieurs pages. |
| [setShowTicks(boolean value)](#setShowTicks-boolean-) | Définit une valeur indiquant s'il faut afficher les marques de repère qui séparent les périodes de temps dans le niveau. |
| [setUnit(int value)](#setUnit-int-) | Définit l'unité d'échelle de temps [TimescaleUnit](../../com.aspose.tasks/timescaleunit) pour le niveau d'échelle de temps. |
| [setUsesFiscalYear(boolean value)](#setUsesFiscalYear-boolean-) | Définit une valeur indiquant s'il faut baser les libellés du niveau sur l'année fiscale. |
### TimescaleTier() {#TimescaleTier--}
```
public TimescaleTier()
```


Initialise une nouvelle instance de la classe [TimescaleTier](../../com.aspose.tasks/timescaletier).

### TimescaleTier(int unit, int count) {#TimescaleTier-int-int-}
```
public TimescaleTier(int unit, int count)
```


Initialise une nouvelle instance de la classe [TimescaleTier](../../com.aspose.tasks/timescaletier).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| unit | int | L'unité d'échelle de temps [TimescaleUnit](../../com.aspose.tasks/timescaleunit). |
| count | int | Le nombre d'unités [TimescaleUnit](../../com.aspose.tasks/timescaleunit). |

### getAlignment() {#getAlignment--}
```
public final int getAlignment()
```


Obtient la façon d'aligner les libellés à l'intérieur de chaque période de temps du niveau ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)).

**Returns:**
int - comment aligner les libellés à l'intérieur de chaque période de temps du niveau ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)).
### getCount() {#getCount--}
```
public final int getCount()
```


Obtient l'intervalle d'unité de temps dans lequel afficher les libellés pour le niveau. La valeur par défaut est 1.

**Returns:**
int - l'intervalle d'unité de temps dans lequel afficher les libellés pour le niveau.
### getDateTimeConverter() {#getDateTimeConverter--}
```
public final DateTimeConverter getDateTimeConverter()
```


Obtient une fonction de rappel pour gérer le rendu du repère de date dans ce niveau.

**Returns:**
[DateTimeConverter](../../com.aspose.tasks/datetimeconverter) - a callback function for handling rendering date tick in this tier.
### getLabel() {#getLabel--}
```
public final int getLabel()
```


Obtient le libellé de date [DateLabel](../../com.aspose.tasks/datelabel) pour le niveau d'échelle de temps.

**Returns:**
int - libellé de date [DateLabel](../../com.aspose.tasks/datelabel) pour le niveau d'échelle de temps.
### getRenderLabelOnEachPage() {#getRenderLabelOnEachPage--}
```
public final boolean getRenderLabelOnEachPage()
```


Obtient le drapeau qui indique si les libellés de date doivent être rendus sur chaque page lorsqu'une période de temps s'étend sur plusieurs pages. Si la valeur est 'true', lorsque la période de temps s'étend sur plusieurs pages, les libellés de date pour la période sont rendus sur chaque page. Si la valeur est 'false', le libellé de date est rendu une seule fois selon la valeur de la propriété `Alignment`([getAlignment](../../com.aspose.tasks/timescaletier\#getAlignment--)/[setAlignment(int)](../../com.aspose.tasks/timescaletier\#setAlignment-int-)).

--------------------

N'a pas d'équivalent dans MS Project.

**Returns:**
booléen - indicateur qui définit si les étiquettes de date doivent être rendues sur chaque page lorsqu'une période s'étend sur plusieurs pages.
### getShowTicks() {#getShowTicks--}
```
public final boolean getShowTicks()
```


Obtient une valeur indiquant s'il faut afficher les marques de repère qui séparent les périodes de temps dans le niveau.

**Returns:**
booléen - une valeur indiquant s'il faut afficher les marques de graduation qui séparent les périodes de temps dans le niveau.
### getUnit() {#getUnit--}
```
public final int getUnit()
```


Obtient l'unité d'échelle de temps [TimescaleUnit](../../com.aspose.tasks/timescaleunit) pour le niveau d'échelle de temps. La valeur par défaut est [TimescaleUnit](../../com.aspose.tasks/timescaleunit).

**Returns:**
int - unité d'échelle de temps [TimescaleUnit](../../com.aspose.tasks/timescaleunit) pour le niveau d'échelle de temps.
### getUsesFiscalYear() {#getUsesFiscalYear--}
```
public final boolean getUsesFiscalYear()
```


Obtient une valeur indiquant s'il faut baser les libellés du niveau sur l'année fiscale.

**Returns:**
booléen - une valeur indiquant s'il faut baser les étiquettes du niveau sur l'année fiscale.
### setAlignment(int value) {#setAlignment-int-}
```
public final void setAlignment(int value)
```


Définit la façon d'aligner les libellés à l'intérieur de chaque période de temps du niveau ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | int | comment aligner les étiquettes à l'intérieur de chaque période de temps du niveau ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)). |

### setCount(int value) {#setCount-int-}
```
public final void setCount(int value)
```


Définit l'intervalle d'unité de temps dans lequel afficher les étiquettes pour le niveau. La valeur par défaut est 1.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | l'intervalle d'unité de temps dans lequel afficher les étiquettes pour le niveau. |

### setDateTimeConverter(DateTimeConverter value) {#setDateTimeConverter-com.aspose.tasks.DateTimeConverter-}
```
public final void setDateTimeConverter(DateTimeConverter value)
```


Définit une fonction de rappel pour gérer le rendu du repère de date dans ce niveau.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | [DateTimeConverter](../../com.aspose.tasks/datetimeconverter) | une fonction de rappel pour gérer le rendu de la graduation de date dans ce niveau. |

### setLabel(int value) {#setLabel-int-}
```
public final void setLabel(int value)
```


Définit le libellé de date [DateLabel](../../com.aspose.tasks/datelabel) pour le niveau d'échelle de temps.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | int | étiquette de date [DateLabel](../../com.aspose.tasks/datelabel) pour le niveau d'échelle de temps. |

### setRenderLabelOnEachPage(boolean value) {#setRenderLabelOnEachPage-boolean-}
```
public final void setRenderLabelOnEachPage(boolean value)
```


Définit le drapeau qui indique si les étiquettes de date doivent être rendues sur chaque page lorsqu'une période s'étend sur plusieurs pages. Si la valeur est 'true', lorsque la période s'étend sur plusieurs pages, les étiquettes de date pour la période sont rendues sur chaque page. Si la valeur est 'false', l'étiquette de date est rendue une seule fois selon la valeur de la propriété `Alignment`([getAlignment](../../com.aspose.tasks/timescaletier\#getAlignment--)/[setAlignment(int)](../../com.aspose.tasks/timescaletier\#setAlignment-int-)).

--------------------

N'a pas d'équivalent dans MS Project.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | drapeau qui indique si les étiquettes de date doivent être rendues sur chaque page lorsqu'une période s'étend sur plusieurs pages. |

### setShowTicks(boolean value) {#setShowTicks-boolean-}
```
public final void setShowTicks(boolean value)
```


Définit une valeur indiquant s'il faut afficher les marques de repère qui séparent les périodes de temps dans le niveau.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant s'il faut afficher les marques de graduation qui séparent les périodes de temps dans le niveau. |

### setUnit(int value) {#setUnit-int-}
```
public final void setUnit(int value)
```


Définit l'unité d'échelle de temps [TimescaleUnit](../../com.aspose.tasks/timescaleunit) pour le niveau d'échelle de temps. La valeur par défaut est [TimescaleUnit](../../com.aspose.tasks/timescaleunit).

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| value | int | unité d'échelle de temps [TimescaleUnit](../../com.aspose.tasks/timescaleunit) pour le niveau d'échelle de temps. |

### setUsesFiscalYear(boolean value) {#setUsesFiscalYear-boolean-}
```
public final void setUsesFiscalYear(boolean value)
```


Définit une valeur indiquant s'il faut baser les libellés du niveau sur l'année fiscale.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant s'il faut baser les étiquettes du niveau sur l'année fiscale. |

