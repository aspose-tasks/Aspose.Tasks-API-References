---
title: "OutlineCode"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente une valeur d'un code de plan."
type: docs
weight: 167
url: /fr/java/com.aspose.tasks/outlinecode/
---

**Inheritance:**
java.lang.Object
```
public class OutlineCode
```

Représente une valeur d'un code de plan.

--------------------

Deux éléments de données sont nécessaires - un pointeur vers la table de code de plan spécifiée par le FieldId, et la valeur spécifiée soit par le ValueId soit par le ValueGuid pointeur vers la liste de valeurs.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [OutlineCode()](#OutlineCode--) | Initialise une nouvelle instance de la classe [OutlineCode](../../com.aspose.tasks/outlinecode). |
| [OutlineCode(OutlineCodeDefinition codeDefinition, OutlineValue outlineValue)](#OutlineCode-com.aspose.tasks.OutlineCodeDefinition-com.aspose.tasks.OutlineValue-) | Initialise une nouvelle instance de la classe [OutlineCode](../../com.aspose.tasks/outlinecode) en utilisant le Outline Code spécifié et l'une de ses valeurs. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getFieldId()](#getFieldId--) | Obtient la valeur numérique du champ personnalisé Id du projet. |
| [getValueGuid()](#getValueGuid--) | Obtient le GUID de la valeur dans la liste de valeurs. |
| [getValueId()](#getValueId--) | Obtient l'Id dans la liste de valeurs associé à la définition de la collection de code de plan. |
| [setFieldId(String value)](#setFieldId-java.lang.String-) | Définit la valeur numérique du champ personnalisé Id du projet. |
| [setValueGuid(String value)](#setValueGuid-java.lang.String-) | Définit le GUID de la valeur dans la liste de valeurs. |
| [setValueId(int value)](#setValueId-int-) | Définit l'Id dans la liste de valeurs associé à la définition de la collection de code de plan. |
### OutlineCode() {#OutlineCode--}
```
public OutlineCode()
```


Initialise une nouvelle instance de la classe [OutlineCode](../../com.aspose.tasks/outlinecode).

### OutlineCode(OutlineCodeDefinition codeDefinition, OutlineValue outlineValue) {#OutlineCode-com.aspose.tasks.OutlineCodeDefinition-com.aspose.tasks.OutlineValue-}
```
public OutlineCode(OutlineCodeDefinition codeDefinition, OutlineValue outlineValue)
```


Initialise une nouvelle instance de la classe [OutlineCode](../../com.aspose.tasks/outlinecode) en utilisant le Outline Code spécifié et l'une de ses valeurs.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| codeDefinition | [OutlineCodeDefinition](../../com.aspose.tasks/outlinecodedefinition) | définition du code de contour. |
| outlineValue | [OutlineValue](../../com.aspose.tasks/outlinevalue) | une des valeurs de définition du code de contour. |

### getFieldId() {#getFieldId--}
```
public final String getFieldId()
```


Obtient la valeur numérique du champ personnalisé Id du projet.

**Returns:**
java.lang.String - la valeur numérique du champ personnalisé Id du projet.
### getValueGuid() {#getValueGuid--}
```
public final String getValueGuid()
```


Obtient le GUID de la valeur dans la liste de valeurs. Le ValueGuid correspond au FieldGuid dans la liste de valeurs.

**Returns:**
java.lang.String - le GUID de la valeur dans la liste de valeurs.
### getValueId() {#getValueId--}
```
public final int getValueId()
```


Obtient l'Id dans la liste de valeurs associé à la définition de la collection de code de plan.

**Returns:**
int - l'Id dans la liste de valeurs associé à la définition dans la collection de code de contour.
### setFieldId(String value) {#setFieldId-java.lang.String-}
```
public final void setFieldId(String value)
```


Définit la valeur numérique du champ personnalisé Id du projet.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | la valeur numérique du champ personnalisé Id du projet. |

### setValueGuid(String value) {#setValueGuid-java.lang.String-}
```
public final void setValueGuid(String value)
```


Définit le GUID de la valeur dans la liste de valeurs. Le ValueGuid correspond au FieldGuid dans la liste de valeurs.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | le GUID de la valeur dans la liste de valeurs. |

### setValueId(int value) {#setValueId-int-}
```
public final void setValueId(int value)
```


Définit l'Id dans la liste de valeurs associé à la définition de la collection de code de plan.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | int | l'Id dans la liste de valeurs associé à la définition dans la collection de code de contour. |

