---
title: "FieldHelper"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Classe d'assistance qui fournit des opérations utiles avec les champs."
type: docs
weight: 88
url: /fr/java/com.aspose.tasks/fieldhelper/
---

**Inheritance:**
java.lang.Object
```
public class FieldHelper
```

Classe d'assistance qui fournit des opérations utiles avec les champs.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [FieldHelper()](#FieldHelper--) |  |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getDefaultFieldTitle(int field)](#getDefaultFieldTitle-int-) | Renvoie un titre par défaut du champ spécifique. |
| [getDefaultTaskFieldTitle(byte taskKey)](#getDefaultTaskFieldTitle-byte-) | Renvoie un titre par défaut du champ de tâche spécifique. |
### FieldHelper() {#FieldHelper--}
```
public FieldHelper()
```


### getDefaultFieldTitle(int field) {#getDefaultFieldTitle-int-}
```
public static String getDefaultFieldTitle(int field)
```


Renvoie un titre par défaut du champ spécifique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| champ | int | Champ pour obtenir un titre par défaut. |

**Returns:**
java.lang.String - Un titre par défaut du champ spécifique si le champ peut être affiché dans la vue de MS Project, sinon null.
### getDefaultTaskFieldTitle(byte taskKey) {#getDefaultTaskFieldTitle-byte-}
```
public static String getDefaultTaskFieldTitle(byte taskKey)
```


Renvoie un titre par défaut du champ de tâche spécifique.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| taskKey | byte | Champ de tâche pour obtenir un titre par défaut. |

**Returns:**
java.lang.String - Un titre par défaut du champ de tâche spécifique si le champ peut être affiché dans la vue de MS Project, sinon null.
