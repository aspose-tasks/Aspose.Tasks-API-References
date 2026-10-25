---
title: "CustomProjectPropertyCollection"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Representa una colección de propiedades personalizadas del proyecto."
type: docs
weight: 61
url: /es/java/com.aspose.tasks/customprojectpropertycollection/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.PropertyCollection, com.aspose.tasks.PropertyKeyedCollection
```
public final class CustomProjectPropertyCollection extends PropertyKeyedCollection<CustomProjectProperty>
```

Representa una colección de propiedades personalizadas del proyecto.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [CustomProjectPropertyCollection()](#CustomProjectPropertyCollection--) | Inicializa una nueva instancia de la clase [CustomProjectPropertyCollection](../../com.aspose.tasks/customprojectpropertycollection). |
## Métodos

| Método | Descripción |
| --- | --- |
| [add(String name, boolean value)](#add-java.lang.String-boolean-) | Crea una nueva propiedad personalizada. |
| [add(String name, double value)](#add-java.lang.String-double-) | Crea una nueva propiedad personalizada. |
| [add(String name, String value)](#add-java.lang.String-java.lang.String-) | Crea una nueva propiedad personalizada. |
| [add(String name, Date value)](#add-java.lang.String-java.util.Date-) | Crea una nueva propiedad personalizada. |
| [clear()](#clear--) | Limpia la PropertyCollection. |
| [isReadOnly()](#isReadOnly--) | Obtiene un valor que indica si esta colección es de solo lectura; de lo contrario, false. |
| [remove(String name)](#remove-java.lang.String-) | Elimina una propiedad con el nombre especificado de la colección. |
### CustomProjectPropertyCollection() {#CustomProjectPropertyCollection--}
```
public CustomProjectPropertyCollection()
```


Inicializa una nueva instancia de la clase [CustomProjectPropertyCollection](../../com.aspose.tasks/customprojectpropertycollection).

### add(String name, boolean value) {#add-java.lang.String-boolean-}
```
public final CustomProjectProperty add(String name, boolean value)
```


Crea una nueva propiedad personalizada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String | El nombre de la propiedad. |
| valor | boolean | El valor del objeto de propiedad recién creado. |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### add(String name, double value) {#add-java.lang.String-double-}
```
public final CustomProjectProperty add(String name, double value)
```


Crea una nueva propiedad personalizada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String | El nombre de la propiedad. |
| valor | double | El valor del objeto de propiedad recién creado. |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### add(String name, String value) {#add-java.lang.String-java.lang.String-}
```
public final CustomProjectProperty add(String name, String value)
```


Crea una nueva propiedad personalizada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String | El nombre de la propiedad. |
| valor | java.lang.String | El valor del objeto de propiedad recién creado. |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### add(String name, Date value) {#add-java.lang.String-java.util.Date-}
```
public final CustomProjectProperty add(String name, Date value)
```


Crea una nueva propiedad personalizada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String | El nombre de la propiedad. |
| valor | java.util.Date | El valor del objeto de propiedad recién creado. |

**Returns:**
[CustomProjectProperty](../../com.aspose.tasks/customprojectproperty) - The newly created property object.
### clear() {#clear--}
```
public final void clear()
```


Limpia la PropertyCollection.

### isReadOnly() {#isReadOnly--}
```
public boolean isReadOnly()
```


Obtiene un valor que indica si esta colección es de solo lectura; de lo contrario, false.

**Returns:**
boolean - un valor que indica si esta colección es de solo lectura; de lo contrario, false.
### remove(String name) {#remove-java.lang.String-}
```
public final boolean remove(String name)
```


Elimina una propiedad con el nombre especificado de la colección.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | java.lang.String | El nombre de la propiedad sin distinción de mayúsculas. |

**Returns:**
boolean - True si el elemento se encuentra y elimina con éxito; de lo contrario, false.
