---
title: "VbaModule"
second_title: "Référence API d'Aspose.Tasks pour Java"
description: "Représente un module VBA."
type: docs
weight: 334
url: /fr/java/com.aspose.tasks/vbamodule/
---

**Inheritance:**
java.lang.Object
```
public final class VbaModule
```

Représente un module VBA.
## Méthodes

| Méthode | Description |
| --- | --- |
| [createClassModule(String name)](#createClassModule-java.lang.String-) | Crée une instance de [VbaModule](../../com.aspose.tasks/vbamodule) avec le type VbaModuleType.ClassModule. |
| [createProceduralModule(String name)](#createProceduralModule-java.lang.String-) | Crée une instance de [VbaModule](../../com.aspose.tasks/vbamodule) avec le type VbaModuleType.ProceduralModule. |
| [getAttributes()](#getAttributes--) | Obtient une collection des attributs du module. |
| [getName()](#getName--) | Obtient le nom du module VBA |
| [getSourceCode()](#getSourceCode--) | Obtient le code source du module VBA |
| [getType()](#getType--) | Obtient le type du module. |
| [setName(String value)](#setName-java.lang.String-) | Un nom du module VBA |
| [setSourceCode(String value)](#setSourceCode-java.lang.String-) | Définit le code source du module VBA |
### createClassModule(String name) {#createClassModule-java.lang.String-}
```
public static VbaModule createClassModule(String name)
```


Crée une instance de [VbaModule](../../com.aspose.tasks/vbamodule) avec le type VbaModuleType.ClassModule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[VbaModule](../../com.aspose.tasks/vbamodule)
### createProceduralModule(String name) {#createProceduralModule-java.lang.String-}
```
public static VbaModule createProceduralModule(String name)
```


Crée une instance de [VbaModule](../../com.aspose.tasks/vbamodule) avec le type VbaModuleType.ProceduralModule.

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[VbaModule](../../com.aspose.tasks/vbamodule)
### getAttributes() {#getAttributes--}
```
public final VbaModuleAttributeCollection getAttributes()
```


Obtient une collection des attributs du module.

**Returns:**
[VbaModuleAttributeCollection](../../com.aspose.tasks/vbamoduleattributecollection) - a collection of the module's attributes.
### getName() {#getName--}
```
public final String getName()
```


Obtient le nom du module VBA

**Returns:**
java.lang.String - un nom du module VBA
### getSourceCode() {#getSourceCode--}
```
public final String getSourceCode()
```


Obtient le code source du module VBA

**Returns:**
java.lang.String - un code source du module VBA
### getType() {#getType--}
```
public final int getType()
```


Obtient le type du module.

**Returns:**
int - le type du module.
### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Un nom du module VBA

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | un nom du module VBA |

### setSourceCode(String value) {#setSourceCode-java.lang.String-}
```
public final void setSourceCode(String value)
```


Définit le code source du module VBA

**Parameters:**
| Paramètre | Type | Description |
| --- | --- | --- |
| valeur | java.lang.String | un code source du module VBA |

