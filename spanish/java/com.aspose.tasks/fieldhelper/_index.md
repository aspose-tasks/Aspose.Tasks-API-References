---
title: "FieldHelper"
second_title: "Referencia de API de Aspose.Tasks para Java"
description: "Clase auxiliar que proporciona operaciones útiles con campos."
type: docs
weight: 88
url: /es/java/com.aspose.tasks/fieldhelper/
---

**Inheritance:**
java.lang.Object
```
public class FieldHelper
```

Clase auxiliar que proporciona operaciones útiles con campos.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [FieldHelper()](#FieldHelper--) |  |
## Métodos

| Método | Descripción |
| --- | --- |
| [getDefaultFieldTitle(int field)](#getDefaultFieldTitle-int-) | Devuelve un título predeterminado del campo específico. |
| [getDefaultTaskFieldTitle(byte taskKey)](#getDefaultTaskFieldTitle-byte-) | Devuelve un título predeterminado del campo de tarea específico. |
### FieldHelper() {#FieldHelper--}
```
public FieldHelper()
```


### getDefaultFieldTitle(int field) {#getDefaultFieldTitle-int-}
```
public static String getDefaultFieldTitle(int field)
```


Devuelve un título predeterminado del campo específico.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| campo | int | Campo para obtener un título predeterminado. |

**Returns:**
java.lang.String - Un título predeterminado del campo específico si el campo puede mostrarse en la vista de MS Project, null en caso contrario.
### getDefaultTaskFieldTitle(byte taskKey) {#getDefaultTaskFieldTitle-byte-}
```
public static String getDefaultTaskFieldTitle(byte taskKey)
```


Devuelve un título predeterminado del campo de tarea específico.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| taskKey | byte | Campo de tarea para obtener un título predeterminado. |

**Returns:**
java.lang.String - Un título predeterminado del campo de tarea específico si el campo puede mostrarse en la vista de MS Project, null en caso contrario.
