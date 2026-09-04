---
title: "PrimaveraSaveOptions"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Permet de spécifier des options supplémentaires lors de l'enregistrement du projet au format Primavera XER."
type: docs
weight: 208
url: /fr/java/com.aspose.tasks/primaverasaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class PrimaveraSaveOptions extends SimpleSaveOptions
```

Permet de spécifier des options supplémentaires lors de l'enregistrement du projet au format Primavera XER.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [PrimaveraSaveOptions()](#PrimaveraSaveOptions--) | Initialise une nouvelle instance de la classe [PrimaveraSaveOptions](../../com.aspose.tasks/primaverasaveoptions). |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getActivityIdIncrement()](#getActivityIdIncrement--) | Obtient l'incrément utilisé lors du renumérotage des ID d'activité. |
| [getActivityIdPrefix()](#getActivityIdPrefix--) | Obtient le préfixe utilisé lors du renumérotage des ID d'activité. |
| [getActivityIdSuffix()](#getActivityIdSuffix--) | Obtient le suffixe utilisé lors du renumérotage des ID d'activité. |
| [getRenumberActivityIds()](#getRenumberActivityIds--) | Obtient une valeur indiquant s'il est nécessaire de renuméroter les ID d'activité. |
| [getSkipSummaryAssignments()](#getSkipSummaryAssignments--) | Obtient une valeur indiquant si les affectations de ressources aux tâches récapitulatives doivent être ignorées lors de l'exportation. |
| [setActivityIdIncrement(int value)](#setActivityIdIncrement-int-) | Définit l'incrément utilisé lors du renumérotage des ID d'activité. |
| [setActivityIdPrefix(String value)](#setActivityIdPrefix-java.lang.String-) | Définit le préfixe utilisé lors du renumérotage des ID d'activité. |
| [setActivityIdSuffix(int value)](#setActivityIdSuffix-int-) | Définit le suffixe utilisé lors du renumérotage des ID d'activité. |
| [setRenumberActivityIds(boolean value)](#setRenumberActivityIds-boolean-) | Définit une valeur indiquant s'il est nécessaire de renuméroter les ID d'activité. |
| [setSkipSummaryAssignments(boolean value)](#setSkipSummaryAssignments-boolean-) | Définit une valeur indiquant si les affectations de ressources aux tâches récapitulatives doivent être ignorées lors de l'exportation. |
### PrimaveraSaveOptions() {#PrimaveraSaveOptions--}
```
public PrimaveraSaveOptions()
```


Initialise une nouvelle instance de la classe [PrimaveraSaveOptions](../../com.aspose.tasks/primaverasaveoptions).

### getActivityIdIncrement() {#getActivityIdIncrement--}
```
public final int getActivityIdIncrement()
```


Obtient l'incrément utilisé lors du renumérotage des ID d'activité.

**Returns:**
int - l'incrément utilisé lors du renumérotage des ID d'activité.
### getActivityIdPrefix() {#getActivityIdPrefix--}
```
public final String getActivityIdPrefix()
```


Obtient le préfixe utilisé lors du renumérotage des ID d'activité.

**Returns:**
java.lang.String - le préfixe utilisé lors du renumérotage des ID d'activité.
### getActivityIdSuffix() {#getActivityIdSuffix--}
```
public final int getActivityIdSuffix()
```


Obtient le suffixe utilisé lors du renumérotage des ID d'activité.

**Returns:**
int - le suffixe utilisé lors du renumérotage des ID d'activité.
### getRenumberActivityIds() {#getRenumberActivityIds--}
```
public final boolean getRenumberActivityIds()
```


Obtient une valeur indiquant s'il est nécessaire de renuméroter les ID d'activité.

**Returns:**
boolean - une valeur indiquant s'il est nécessaire de renuméroter les ID d'activité.
### getSkipSummaryAssignments() {#getSkipSummaryAssignments--}
```
public final boolean getSkipSummaryAssignments()
```


Obtient une valeur indiquant si les affectations de ressources aux tâches récapitulatives doivent être ignorées lors de l'exportation.

Le logiciel Primavera ne prend pas en charge l'affectation de ressources aux tâches de synthèse (WBS). Ainsi, l'exportation de ces affectations peut entraîner un fichier invalide selon le modèle de Primavera. Si vrai, les affectations aux tâches de synthèse sont ignorées lors de l'exportation. Si faux (valeur par défaut), une exception sera levée si une affectation à une tâche de synthèse est rencontrée lors de l'exportation.

**Returns:**
booléen - une valeur indiquant si les affectations de ressources aux tâches de synthèse doivent être ignorées lors de l'exportation.
### setActivityIdIncrement(int value) {#setActivityIdIncrement-int-}
```
public final void setActivityIdIncrement(int value)
```


Définit l'incrément utilisé lors du renumérotage des ID d'activité.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | l'incrément utilisé lors du renumérotage des ID d'activité. |

### setActivityIdPrefix(String value) {#setActivityIdPrefix-java.lang.String-}
```
public final void setActivityIdPrefix(String value)
```


Définit le préfixe utilisé lors du renumérotage des ID d'activité.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | le préfixe utilisé lors du renumérotage des ID d'activité. |

### setActivityIdSuffix(int value) {#setActivityIdSuffix-int-}
```
public final void setActivityIdSuffix(int value)
```


Définit le suffixe utilisé lors du renumérotage des ID d'activité.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | le suffixe utilisé lors du renumérotage des ID d'activité. |

### setRenumberActivityIds(boolean value) {#setRenumberActivityIds-boolean-}
```
public final void setRenumberActivityIds(boolean value)
```


Définit une valeur indiquant s'il est nécessaire de renuméroter les ID d'activité.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant s'il est nécessaire de renuméroter les ID d'activité. |

### setSkipSummaryAssignments(boolean value) {#setSkipSummaryAssignments-boolean-}
```
public final void setSkipSummaryAssignments(boolean value)
```


Définit une valeur indiquant si les affectations de ressources aux tâches récapitulatives doivent être ignorées lors de l'exportation.

Le logiciel Primavera ne prend pas en charge l'affectation de ressources aux tâches de synthèse (WBS). Ainsi, l'exportation de ces affectations peut entraîner un fichier invalide selon le modèle de Primavera. Si vrai, les affectations aux tâches de synthèse sont ignorées lors de l'exportation. Si faux (valeur par défaut), une exception sera levée si une affectation à une tâche de synthèse est rencontrée lors de l'exportation.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | booléen | une valeur indiquant si les affectations de ressources aux tâches de synthèse doivent être ignorées lors de l'exportation. |

