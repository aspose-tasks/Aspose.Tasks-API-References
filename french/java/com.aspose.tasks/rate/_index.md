---
title: "Taux"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente une définition d'une période de temps et des tarifs applicables à une ressource pendant cette période."
type: docs
weight: 232
url: /fr/java/com.aspose.tasks/rate/
---

**Inheritance:**
java.lang.Object
```
public class Rate
```

Représente une définition d'une période de temps et des tarifs applicables à une ressource pendant cette période.
## Méthodes

| Méthode | Description |
| --- | --- |
| [getCostPerUse()](#getCostPerUse--) | Obtient le coût par utilisation d'une ressource. |
| [getOvertimeRate()](#getOvertimeRate--) | Obtient le taux d'heures supplémentaires par heure pour une ressource. |
| [getOvertimeRateFormat()](#getOvertimeRateFormat--) | Obtient les unités utilisées par Microsoft Project pour afficher le taux d'heures supplémentaires. |
| [getRateTable()](#getRateTable--) | Obtient l'identifiant unique d'une table de taux pour une ressource. |
| [getRatesFrom()](#getRatesFrom--) | Obtient la date à laquelle un taux devient effectif. |
| [getRatesTo()](#getRatesTo--) | Obtient la dernière date à laquelle un taux est effectif. |
| [getStandardRate()](#getStandardRate--) | Obtient le taux standard par heure pour une ressource. |
| [getStandardRateFormat()](#getStandardRateFormat--) | Obtient les unités utilisées par Microsoft Project pour afficher le taux standard. |
| [setCostPerUse(BigDecimal value)](#setCostPerUse-java.math.BigDecimal-) | Définit le coût par utilisation d'une ressource. |
| [setOvertimeRate(BigDecimal value)](#setOvertimeRate-java.math.BigDecimal-) | Définit le taux d'heures supplémentaires par heure pour une ressource. |
| [setOvertimeRateFormat(int value)](#setOvertimeRateFormat-int-) | Définit les unités utilisées par Microsoft Project pour afficher le taux d'heures supplémentaires. |
| [setRateTable(int value)](#setRateTable-int-) | Définit l'identifiant unique d'un tableau de taux pour une ressource. |
| [setRatesFrom(Date value)](#setRatesFrom-java.util.Date-) | Définit la date à laquelle un taux devient effectif. |
| [setRatesTo(Date value)](#setRatesTo-java.util.Date-) | Définit la dernière date à laquelle un taux est effectif. |
| [setStandardRate(BigDecimal value)](#setStandardRate-java.math.BigDecimal-) | Définit le taux standard par heure pour une ressource. |
| [setStandardRateFormat(int value)](#setStandardRateFormat-int-) | Définit les unités utilisées par Microsoft Project pour afficher le taux standard. |
### getCostPerUse() {#getCostPerUse--}
```
public final BigDecimal getCostPerUse()
```


Obtient le coût par utilisation d'une ressource. Cette valeur est récupérée à partir de la date actuelle si un tableau de taux existe pour une ressource.

**Returns:**
java.math.BigDecimal - le coût par utilisation d'une ressource.
### getOvertimeRate() {#getOvertimeRate--}
```
public final BigDecimal getOvertimeRate()
```


Obtient le taux d'heures supplémentaires par heure pour une ressource.

**Returns:**
java.math.BigDecimal - le taux d'heures supplémentaires par heure pour une ressource.
### getOvertimeRateFormat() {#getOvertimeRateFormat--}
```
public final int getOvertimeRateFormat()
```


Obtient les unités utilisées par Microsoft Project pour afficher le taux d'heures supplémentaires.

**Returns:**
int - les unités utilisées par Microsoft Project pour afficher le taux d'heures supplémentaires.
### getRateTable() {#getRateTable--}
```
public final int getRateTable()
```


Obtient l'identifiant unique d'une table de taux pour une ressource.

**Returns:**
int - l'identifiant unique d'un tableau de taux pour une ressource.
### getRatesFrom() {#getRatesFrom--}
```
public final Date getRatesFrom()
```


Obtient la date à laquelle un taux devient effectif.

**Returns:**
java.util.Date - la date à laquelle un taux devient effectif.
### getRatesTo() {#getRatesTo--}
```
public final Date getRatesTo()
```


Obtient la dernière date à laquelle un taux est effectif.

**Returns:**
java.util.Date - la dernière date à laquelle un taux est effectif.
### getStandardRate() {#getStandardRate--}
```
public final BigDecimal getStandardRate()
```


Obtient le taux standard par heure pour une ressource.

**Returns:**
java.math.BigDecimal - le taux standard par heure pour une ressource.
### getStandardRateFormat() {#getStandardRateFormat--}
```
public final int getStandardRateFormat()
```


Obtient les unités utilisées par Microsoft Project pour afficher le taux standard.

**Returns:**
int - les unités utilisées par Microsoft Project pour afficher le taux standard.
### setCostPerUse(BigDecimal value) {#setCostPerUse-java.math.BigDecimal-}
```
public final void setCostPerUse(BigDecimal value)
```


Définit le coût par utilisation d'une ressource. Cette valeur est récupérée à partir de la date actuelle si un tableau de taux existe pour une ressource.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.math.BigDecimal | le coût par utilisation d'une ressource. |

### setOvertimeRate(BigDecimal value) {#setOvertimeRate-java.math.BigDecimal-}
```
public final void setOvertimeRate(BigDecimal value)
```


Définit le taux d'heures supplémentaires par heure pour une ressource.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.math.BigDecimal | le taux d'heures supplémentaires par heure pour une ressource. |

### setOvertimeRateFormat(int value) {#setOvertimeRateFormat-int-}
```
public final void setOvertimeRateFormat(int value)
```


Définit les unités utilisées par Microsoft Project pour afficher le taux d'heures supplémentaires.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | les unités utilisées par Microsoft Project pour afficher le taux d'heures supplémentaires. |

### setRateTable(int value) {#setRateTable-int-}
```
public final void setRateTable(int value)
```


Définit l'identifiant unique d'un tableau de taux pour une ressource.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | l'identifiant unique d'un tableau de taux pour une ressource. |

### setRatesFrom(Date value) {#setRatesFrom-java.util.Date-}
```
public final void setRatesFrom(Date value)
```


Définit la date à laquelle un taux devient effectif.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.Date | la date à laquelle un taux devient effectif. |

### setRatesTo(Date value) {#setRatesTo-java.util.Date-}
```
public final void setRatesTo(Date value)
```


Définit la dernière date à laquelle un taux est effectif.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.util.Date | la dernière date à laquelle un taux est effectif. |

### setStandardRate(BigDecimal value) {#setStandardRate-java.math.BigDecimal-}
```
public final void setStandardRate(BigDecimal value)
```


Définit le taux standard par heure pour une ressource.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.math.BigDecimal | le taux standard par heure pour une ressource. |

### setStandardRateFormat(int value) {#setStandardRateFormat-int-}
```
public final void setStandardRateFormat(int value)
```


Définit les unités utilisées par Microsoft Project pour afficher le taux standard.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | les unités utilisées par Microsoft Project pour afficher le taux standard. |

