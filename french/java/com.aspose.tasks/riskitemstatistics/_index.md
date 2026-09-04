---
title: "RiskItemStatistics"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente un élément qui stocke les données statistiques pour la tâche du projet analysé."
type: docs
weight: 265
url: /fr/java/com.aspose.tasks/riskitemstatistics/
---

**Inheritance:**
java.lang.Object
```
public class RiskItemStatistics
```

Représente un élément qui stocke les données statistiques pour la tâche du projet analysé.
## Méthodes

| Méthode | Description |
| --- | --- |
| [getExpectedValue()](#getExpectedValue--) | Obtient la valeur attendue de l'élément de risque. |
| [getItemType()](#getItemType--) | Obtient une instance de l'énumération [RiskItemType](../../com.aspose.tasks/riskitemtype). |
| [getMaximum()](#getMaximum--) | Obtient la valeur maximale qui a été générée lors de la simulation Monte Carlo. |
| [getMinimum()](#getMinimum--) | Obtient la valeur minimale qui a été générée lors de la simulation Monte Carlo. |
| [getPercentile(int percent)](#getPercentile-int-) | Obtient une valeur en dessous de laquelle un pourcentage spécifié d'échantillons générés tombe. |
| [getStandardDeviation()](#getStandardDeviation--) | Obtient l'écart type de l'élément de risque. |
| [toString()](#toString--) | Renvoie une représentation courte sous forme de chaîne de l'élément de risque. |
### getExpectedValue() {#getExpectedValue--}
```
public final Date getExpectedValue()
```


Obtient la valeur attendue de l'élément de risque.

**Returns:**
java.util.Date - la valeur attendue de l'élément de risque.
### getItemType() {#getItemType--}
```
public final int getItemType()
```


Obtient une instance de l'énumération [RiskItemType](../../com.aspose.tasks/riskitemtype).

**Returns:**
int - une instance de l'énumération [RiskItemType](../../com.aspose.tasks/riskitemtype).
### getMaximum() {#getMaximum--}
```
public final Date getMaximum()
```


Obtient la valeur maximale qui a été générée lors de la simulation Monte Carlo.

**Returns:**
java.util.Date - la valeur maximale qui a été générée lors de la simulation Monte Carlo.
### getMinimum() {#getMinimum--}
```
public final Date getMinimum()
```


Obtient la valeur minimale qui a été générée lors de la simulation Monte Carlo.

**Returns:**
java.util.Date - la valeur minimale qui a été générée lors de la simulation Monte Carlo.
### getPercentile(int percent) {#getPercentile-int-}
```
public final Date getPercentile(int percent)
```


Obtient une valeur en dessous de laquelle un pourcentage spécifié d'échantillons générés tombe.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| pourcentage | int | le pourcentage spécifié entre 0 et 100. |

**Returns:**
java.util.Date - une valeur en dessous de laquelle un pourcentage spécifié d'échantillons générés se situe.
### getStandardDeviation() {#getStandardDeviation--}
```
public final Duration getStandardDeviation()
```


Obtient l'écart type de l'élément de risque.

**Returns:**
[Duration](../../com.aspose.tasks/duration) - the standard deviation of the risk item.
### toString() {#toString--}
```
public String toString()
```


Renvoie une représentation sous forme de chaîne courte d'un élément de risque. Les détails exacts de la représentation ne sont pas spécifiés et peuvent changer.

**Returns:**
java.lang.String - chaîne courte qui représente l'objet RiskItem.
